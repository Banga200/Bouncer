<template>
  <div class="container">
    <div class="row my-5">
      <div class="col-md-12">
        <div class="table-responsive">
          <table class="table">
            <thead>
              <tr>
                <th></th>
                <th>{{ $t("cart_product_title") }}</th>
                <th></th>
                <th>{{ $t("cart_price_title") }}</th>
                <th>{{ $t("cart_qty_title") }}</th>
                <th>{{ $t("cart_unit_title") }}</th>
              </tr>
            </thead>
            <tbody class="my-5">
              <tr v-for="item in cart.getCartItems" :key="item.id">
                <td>
                  <Icon
                    @click="cart.removeFromCart(item)"
                    class="icon text-danger align-self-center"
                    name="material-symbols:remove-shopping-cart"
                  ></Icon>
                </td>
                <td>
                  <img
                    :src="item.image"
                    class="fluid rounded"
                    width="60"
                    height="60"
                    :alt="item.name"
                  />
                </td>
                <td>
                  {{ item.title }}
                </td>
                <td>${{ item.price }}</td>
                <td class="text-start">
                  <span class="bg-light-subtle d-flex align-items-center">
                    <Icon
                      @click="cart.decrementQ(item)"
                      class="icon"
                      name="ep:minus"
                    ></Icon>
                    {{ item.quantity }}
                    <Icon
                      @click="cart.incrementQ(item)"
                      class="icon"
                      name="ep:plus"
                    ></Icon>
                  </span>
                </td>

                <td>${{ item.price * item.quantity }}</td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>

    <div class="bg-light-subtle ms-md-auto w-25 p-5 justify-content-end my-5">
      <p>
        <span class="text-dark fw-bold d-flex justify-content-between"
          >{{ $t("cart_subtotal") }}
          <h5 class="text-danger">
            ${{
              cart.cartItems
                .reduce((acc, item) => (acc += item.price * item.quantity), 0)
                .toFixed(2)
            }}
          </h5></span
        >
      </p>
      <p class="d-flex text-dark fw-bold d-flex justify-content-between">
        {{ $t("cart_shipping_fee") }} <span class="h5 text-danger"> $20</span>
      </p>
      <p
        class="border-bottom pb-3 text-dark fw-bold d-flex justify-content-between"
      >
        {{ $t("cart_coupon") }} <span class="h5 mx-5">No</span>
      </p>
      <h2 class="d-flex justify-content-between">
        {{ $t("cart_total") }}
        <span>
          ${{
            cart.cartItems
              .reduce(
                (acc, item) => (acc += item.price * item.quantity + 20),
                0
              )
              .toFixed(2)
          }}
        </span>
      </h2>
    </div>
  </div>
</template>

<script setup>
import { useCartStore } from "~/stores/cart";

const cart = useCartStore();
useHead({
  titleTemplate: "Bouncer - Cart",
});
</script>

<style scoped>
.icon {
  cursor: pointer;
  font-size: 10px;
  margin: 0 5px;
}
</style>
