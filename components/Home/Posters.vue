<template>
  <div class="container posters">
    <div class="card-group">
      <div class="card position-relative border-0 first-post">
        <div class="card-body w-75 text-light p-3 mt-3">
          <h5 class="card-title">iPhone 6</h5>
          <p class="card-text">
            Lorem Ipsum dolor sit amet, consectetur adipiscing elit, labor
          </p>
          <h5>$399</h5>
        </div>
        <img
          class="position-absolute w-75"
          src="@/assets/images/poster-1.png"
          alt=""
        />
      </div>
      <div class="card border-0">
        <div class="card-body text-center second-poster">
          <img
            class="mt-3 w-75 h-75"
            src="@/assets/images/poster-2.png"
            alt=""
          />
          <span class="card-footer border-0 bg-white d-flex">
            <h5 class="me-auto">Oculus Rift</h5>
            <h5 class="text-secondary">$349</h5>
          </span>
        </div>
      </div>
      <div
        class="card position-relative border-0 bg-secondary-subtle p-3 d-flex third-poster"
      >
        <div class="card-body w-75">
          <h5 class="card-title">GoPro Hero 6</h5>
          <p class="card-text">
            Lorem Ipsum dolor sit amet, consectetur adipiscing elit, labor
          </p>
          <p class="display-6">$299</p>
        </div>
        <img
          class="position-absolute w-50 h-50"
          src="@/assets/images/poster-3.png"
          alt=""
        />
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style lang="scss" scoped>
.first-post {
  background-color: #ff6875;
  height: 280px;
}
.first-post img {
  bottom: 0;
  right: 0;
}
.second-poster img {
  margin: 0 auto;
}

.third-poster img {
  right: 0;
  bottom: 0;
  margin-bottom: 15px;
}
@media (min-width: 575px) {
  .posters {
    margin-top: -125px;
    margin-bottom: 150px;
  }
}
</style>
