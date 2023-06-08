<template>
  <div class="container footer-contain">
    <div class="row">
      <div class="col-sm-12 col-md-6 col-lg-4">
        <h1 class="text-body-secondary mb-3">{{ $t("brand_title") }}</h1>
        <p>
          {{ $t("header_title_content") }}
        </p>
      </div>
      <div class="col-sm-12 col-md-6 col-lg-4">
        <h6 class="my-3">{{ $t("follow_title") }}</h6>
        <p class="my-4">
          {{ $t("follow_content") }}
        </p>
        <div class="icons d-flex">
          <Icon name="fa6-brands:facebook-f" class="text-primary mx-5 fs-4" />
          <Icon name="devicon:twitter" class="fs-4" />
        </div>
      </div>
      <div class="col-sm-12 col-md-6 col-lg-4">
        <h6 class="my-3">{{ $t("contact_title") }}</h6>
        <p class="my-4">
          {{ $t("contact_content") }}
        </p>
      </div>
    </div>
    <div class="row mt-5">
      <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 my-4">
        <h5 class="text-center text-md-start">{{ $t("information_title") }}</h5>
        <ul class="list-group list-group-flush text-center text-md-start">
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("about_us") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("information_title") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("privacy_link") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("terms_link") }}
            </a>
          </li>
        </ul>
      </div>
      <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 my-4">
        <h5 class="text-center text-md-start">{{ $t("service_title") }}</h5>
        <ul class="list-group list-group-flush text-center text-md-start">
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("about_us") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("information_title") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("privacy_link") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("terms_link") }}
            </a>
          </li>
        </ul>
      </div>
      <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 my-4">
        <h5 class="text-center text-md-start">{{ $t("extra_title") }}</h5>
        <ul class="list-group list-group-flush text-center text-md-start">
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("about_us") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("information_title") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("privacy_link") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("terms_link") }}
            </a>
          </li>
        </ul>
      </div>
      <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 my-4">
        <h5 class="text-center text-md-start">{{ $t("my_account") }}</h5>
        <ul class="list-group list-group-flush text-center text-md-start">
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("about_us") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("information_title") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("privacy_link") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("terms_link") }}
            </a>
          </li>
        </ul>
      </div>
      <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 my-4">
        <h5 class="text-center text-md-start">{{ $t("userful_link") }}</h5>
        <ul class="list-group list-group-flush text-center text-md-start">
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("about_us") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("information_title") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("privacy_link") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("terms_link") }}
            </a>
          </li>
        </ul>
      </div>
      <div class="col-xs-12 col-sm-6 col-md-4 col-lg-3 col-xl-2 my-4">
        <h5 class="text-center text-md-start">{{ $t("offer_title") }}</h5>
        <ul class="list-group list-group-flush text-center text-md-start">
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("about_us") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("information_title") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("privacy_link") }}
            </a>
          </li>
          <li class="list-group-item border-0">
            <a href="#" class="text-decoration-none text-dark"
              >{{ $t("terms_link") }}
            </a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script setup></script>

<style scoped>
.footer-contain {
  margin-top: 125px;
}
</style>
