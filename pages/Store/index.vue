<template>
  <div class="container mt-5">
    <div class="row justify-content-between d-flex flex-md-row flex-column">
      <div class="col-12 col-sm-7 col-md-5 col-lg-4 col-xl-3 mb-5">
        <div class="list-group bg-light-subtle text-first ps-2">
          <h3 class="my-3 mx-auto">{{ $t("home_store") }}</h3>
          <a
            @click="store.getProducts({ limit: 20 })"
            class="list-group-item list-group-item-action bg-light-subtle list-group-item-tertiary border-0"
            >{{ $t("all_items") }}</a
          >
          <a
            v-for="cate in store.categories"
            @click="store.getProductsCategory(cate)"
            :key="cate.id"
            class="list-group-item list-group-item-action text-capitalize bg-light-subtle list-group-item-tertiary border-0"
            >{{ $t(cate) }}</a
          >
        </div>

        <Range @rangeChanged="filterProducts" />
      </div>
      <div class="card-group col-xl-9">
        <div
          class="row justify-content-center justify-content-sm-around mb-5 text-center"
        >
          <div
            v-for="product in store.products"
            :key="product.id"
            class="col-sm-5 col-md-4 col-lg-4"
          >
            <NuxtLink
              style="width: 230px; height: 249px"
              :to="`/store/${product.id}`"
              class="card shadow text-decoration-none mx-auto col-lg-1 text-center my-5"
            >
              <img
                :src="`${product.image}`"
                class="card-img-top mx-auto mt-3 h-50 w-50"
                alt="..."
              />
              <div class="card-body h-50">
                <h6 class="card-title" style="font-size: 13px">
                  {{ product.title }}
                </h6>
                <p class="card-text text-danger">$ {{ product.price }}</p>
              </div>
            </NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { useProductStore } from "~/stores/product";

const store = useProductStore();
useHead({
  titleTemplate: "Bouncer - Store",
});

onMounted(() => {
  store.getProducts({ limit: 20 });
});
</script>

<style scoped>
.list-group a {
  cursor: pointer;
}
</style>
