<script setup>
import RotatingCard from "../../../examples/cards/rotatingCards/RotatingCard.vue";
import RotatingCardFront from "../../../examples/cards/rotatingCards/RotatingCardFront.vue";
import RotatingCardBack from "../../../examples/cards/rotatingCards/RotatingCardBack.vue";
import DefaultInfoCard from "../../../examples/cards/infoCards/DefaultInfoCard.vue";
</script>
<template>
  <section class="my-5 py-5">
    <div class="container">
      <div class="row align-items-center">
        <div class="col-lg-4 ms-auto me-auto p-lg-4 mt-lg-0 mt-4">
          <RotatingCard>
            <RotatingCardFront
              image="https://images.unsplash.com/photo-1569683795645-b62e50fbf103?ixlib=rb-1.2.1&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=987&q=80"
              icon="touch_app"
              title="Feel the <br /> Material Kit"
              description="All the Bootstrap components that you need in a development have been
        re-design with the new look."
            />

            <RotatingCardBack
              image="https://images.unsplash.com/photo-1498889444388-e67ea62c464b?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=1365&q=80"
              title="Discover More"
              description="You will save a lot of time going from prototyping to full-functional
                code because all elements are implemented."
              :action="[
                {
                  route: './/sections/page-sections/hero-sections.html',
                  label: 'Start with Headers',
                },
              ]"
            />
          </RotatingCard>
        </div>
        <div class="col-lg-6 ms-auto">
          <div class="row justify-content-start">
            <DefaultInfoCard
              icon="folder_shared"
              title="免費提供個案諮詢"
              description="提供房東免費個案諮詢，協助資產活化、提升租⾦"
            />
            <DefaultInfoCard
              icon="brightness_4"
              title="房東管理不間斷"
              description="24⼩時房東專線房務管理不中斷"
            />
          </div>
          <div class="row justify-content-start mt-5">
            <DefaultInfoCard
              class="mt-3"
              icon="home"
              title="保障屋主收租權益"
              description="代理逾期收租服務，社區現場守候，加強保障屋主收租權益"
            />
            <DefaultInfoCard
              class="mt-3"
              icon="thumb_up"
              title="專業合作廠商"
              description="⽔電、⽊⼯、油漆、家具、家電、衛浴與修繕協⼒廠商⼀應俱全"
            />
            <DefaultInfoCard
              class="mt-3"
              icon="favorite"
              title="安⼼素質保障"
              description="業務+屋主雙層鑑定優質房客，多⼀層保護與⽤⼼"
            />
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
