<template>
  <div class="container mx-auto px-4">
    <FloralHeading>Wedding Details</FloralHeading>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-4">
      <div>
        <p class="text-lg mb-1"><b>Ceremony</b></p>
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m14!1m8!1m3!1d11951.104934376746!2d-82.0208439!3d41.5091237!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x88308f966ea8361f%3A0xeab3dbbc03308729!2sAvon%20Lake%20United%20Church%20of%20Christ!5e0!3m2!1sen!2sus!4v1680916356907!5m2!1sen!2sus"
          width="100%"
          height="450"
          style="border: 0"
          allowfullscreen="false"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        ></iframe>
        <p class="mb-0">
          <i class="fa-solid fa-location-dot me-2"></i
          ><em>Avon Lake United Church of Christ</em>
        </p>
        <a
          class="text-slate-500"
          href="https://goo.gl/maps/k8MXS8hkPntpeTBy5?coh=178571&entry=tt"
        >
          32801 Electric Blvd<br />Avon Lake, OH 44012
        </a>
        <p><i class="fa-solid fa-clock me-2"></i>3:30 PM</p>
      </div>
      <div>
        <p class="text-lg mb-1"><b>Reception</b></p>
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2988.2804172433107!2d-81.70886642351093!3d41.49819767128599!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x8830f063da81cf83%3A0xaa03090d60845068!2sMusic%20Box%20Supper%20Club!5e0!3m2!1sen!2sus!4v1680916463710!5m2!1sen!2sus"
          width="100%"
          height="450"
          style="border: 0"
          allowfullscreen="false"
          loading="lazy"
          referrerpolicy="no-referrer-when-downgrade"
        ></iframe>
        <p class="mb-0">
          <em
            ><i class="fa-solid fa-location-dot me-2"></i>Music Box Supper
            Club</em
          >
        </p>
        <a
          class="text-slate-500"
          href="https://goo.gl/maps/m4bCHDSHsdVkRjwb8?coh=178571&entry=tt"
        >
          1148 Main Ave<br />Cleveland, OH 44113
        </a>
        <p class="mb-1"><i class="fa-solid fa-clock me-2"></i>5:30 PM</p>
        <p>* Valet parking provided</p>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import FloralHeading from '~/components/shared/FloralHeading.vue';
</script>
