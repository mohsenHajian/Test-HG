<template>
  <div
    class="flex flex-col mx-auto mt-[92px] md:mt-14 lg:mt-16 xl:mt-[92px] new-landing-container"
  >
    <header class="mb-9 lg:mb-7 xl:mb-[52px]">
      <h2 class="text-base-content text-xl md:text-2xl text-center m-0">
        {{ 'gftfhgtfhtfgh' }}
      </h2>
    </header>
    <div class="grid ss:grid-cols-2 lg:grid-cols-4 gap-5">
      <div
        v-for="step in whyHitalkiSteps"
        :key="step.index"
        class="flex items-center justify-center flex-col relative"
      >
        <!-- <nuxt-img
          loading="lazy"
          class="w-fit h-fit lg:h-[130px]"
          style="flex: 1"
          :src="step.img"
        /> -->
        <img
          class="w-fit h-fit lg:h-[130px]"
          style="flex: 1"
          :src="step.img"
        />
        <h4
          class="text-primary-dark-gray text-center lg:my-my-3 xl:my-4 text-xl sm:text-lg md:text-lg xl:text-xl IranSansMedium"
        >
          {{ step.title }}
        </h4>
        <p
          class="leading-normal text-sm lg:text-xs xl:text-sm text-center text-gray-dark IranSansMedium lg:min-h-[80px]"
          style="word-spacing: -1px"
        >
          {{ step.description }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      whyHitalkiSteps: [
        {
          index: 1,
          title: "this.$t('newwhyhitalki.one.title')",
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit eum quae esse veniam beatae iste corrupti laudantium obcaecati, fugit quia.",
          img: "/newWhyHitalki/reason-1.gif",
        },
        {
          index: 2,
          title: "this.$t('newwhyhitalki.two.title')",
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit eum quae esse veniam beatae iste corrupti laudantium obcaecati, fugit quia.",
          img: "/newWhyHitalki/reason-2.gif",
        },
        {
          index: 3,
          title: "this.$t('newwhyhitalki.three.title')",
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit eum quae esse veniam beatae iste corrupti laudantium obcaecati, fugit quia.",
          img: "/newWhyHitalki/reason-3.gif",
        },
        {
          index: 4,
          title: "this.$t('newwhyhitalki.four.title')",
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Velit eum quae esse veniam beatae iste corrupti laudantium obcaecati, fugit quia.",
          img: "/newWhyHitalki/reason-4.gif",
        },
      ],
    };
  },
};
</script>
