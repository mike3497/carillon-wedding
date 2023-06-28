<template>
  <div>
    <HeroImage />

    <div class="container mx-auto max-w-xl px-4 mb-4">
      <FloralHeading>{{ daysUntilWedding }}</FloralHeading>
      <p>
        Welcome to our wedding website! We are thrilled to share our love story
        and journey with you as we embark on this new chapter in our lives. This
        website is designed to be a one-stop-shop for all the information you
        will need about our wedding day. From our story and proposal to the
        details of the ceremony and reception, we want to ensure that our guests
        have all the information they need to join us in celebrating our love.
        We are grateful for your love and support, and we can't wait to share
        this special day with you!
      </p>
    </div>
    <div class="container mx-auto max-w-xl px-4 mb-4">
      <FloralHeading>Itinerary</FloralHeading>
      <p>Saturday July 22nd, 2023</p>
      <div class="grid grid-cols-2 gap-4">
        <div>
          <h1 class="text-xl font-bold">Ceremony</h1>
          <p class="mb-0"><em>Avon Lake United Church of Christ</em></p>
          <a
            class="text-slate-500"
            href="https://goo.gl/maps/k8MXS8hkPntpeTBy5?coh=178571&entry=tt"
          >
            32801 Electric Blvd<br />Avon Lake, OH 44012
          </a>
          <p>Begins at 3:30 PM</p>
        </div>
        <div>
          <h1 class="text-xl font-bold">Reception</h1>
          <p class="mb-0"><em>Music Box Supper Club</em></p>
          <a
            class="text-slate-500"
            href="https://goo.gl/maps/m4bCHDSHsdVkRjwb8?coh=178571&entry=tt"
          >
            1148 Main Ave<br />Cleveland, OH 44113
          </a>
          <p>Cocktail Hour at 5:30 PM</p>
        </div>
      </div>
    </div>
    <div class="container mx-auto max-w-xl px-4">
      <FloralHeading>Questions?</FloralHeading>
      <p>
        Contact Michael at
        <a class="text-slate-500" href="tel:330-703-7919">(330) 703-7919</a>
        or
        <a class="text-slate-500" href="mailto:mcarillon97@gmail.com"
          >mcarillon97@gmail.com</a
        >
        for any further questions.
      </p>
    </div>
  </div>
</template>

<script setup lang="ts">
import { computed } from 'vue';
import HeroImage from '~/components/HeroImage.vue';
import FloralHeading from '~/components/shared/FloralHeading.vue';

const daysUntilWedding = computed<string>(() => {
  const weddingDate = new Date('2023-07-22');
  const today = new Date();
  const timeDifference = weddingDate.getTime() - today.getTime();
  const daysUntil = Math.ceil(timeDifference / (1000 * 3600 * 24));
  return `${daysUntil} days to go!`;
});
</script>
