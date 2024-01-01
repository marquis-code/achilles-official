<template>
  <main>
    <header-section />
    <LatestVideos />
    <why-achilles />
    <students-questions />
    <lecture-banks />
    <practice-questions />
    <community-members />
    <students-review />
    <frequently-asked-questions />
    <ambassador-section />
    <contact-us />
    <footer-section />
  </main>
</template>

<script>
import HeaderSection from '~/components/HeaderSection.vue';
import LatestVideos from '@/components/LatestVideos.vue';
import WhyAchilles from '@/components/WhyAchilles.vue';
import StudentsQuestions from '@/components/StudentsQuestions.vue';
import LectureBanks from '@/components/LectureBanks.vue';
import PracticeQuestions from '@/components/PracticeQuestions.vue';
import CommunityMembers from '@/components/CommunityMembers.vue';
import StudentsReview from '@/components/StudentsReview.vue';
import FrequentlyAskedQuestions from '@/components/FrequentlyAskedQuestions.vue';
import AmbassadorSection from '@/components/AmbassadorSection.vue';
import ContactUs from '@/components/ContactUs.vue';
import FooterSection from '@/components/FooterSection.vue';
export default {
  components: {
    HeaderSection,
    LatestVideos,
    WhyAchilles,
    StudentsQuestions,
    LectureBanks,
    PracticeQuestions,
    CommunityMembers,
    StudentsReview,
    FrequentlyAskedQuestions,
    AmbassadorSection,
    ContactUs,
    FooterSection
  },
  name: "IndexPage",
};
</script>
