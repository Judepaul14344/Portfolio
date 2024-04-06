<script>
export default {
  setup() {
    return {
      bios: [
        {
          id: 1,
          bio: "Hello, I'm Jude Paul—a melody enthusiast with a heart for technology and a soft spot for our furry friends. Singing and playing instruments are my sanctuary, where I pour my emotions into every note, while caring for and feeding dogs brings me boundless joy and fulfillment. Alongside my passion for music and canine companionship, I'm carving my path as an aspiring IT student, diving into the depths of coding and networking with eagerness and curiosity. Each strum of a chord and each line of code written marks a step forward on my journey of self-discovery and growth, shaping me into a harmonious blend of creativity and technical expertise.",
        },
      ],
    };
  },
};
</script>

<template>
  <div class="block sm:flex sm:gap-10 mt-10 sm:mt-20">
    <!-- About profile image -->
    <div class="w-full sm:w-1/4 mb-7 sm:mb-0">
      <img src="@/assets/images/profile.jpg" class="rounded-xl w-96" alt="" />
    </div>

    <!-- About details -->
    <div class="w-full sm:w-3/4 text-left">
      <p
        v-for="bio in bios"
        :key="bio.id"
        class="font-general-regular mb-4 text-ternary-dark dark:text-ternary-light text-lg"
      >
        {{ bio.bio }}
      </p>
    </div>
  </div>
</template>
