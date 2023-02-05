<script lang="ts">
  import PageHeader from "$lib/components/PageHeader.svelte";
  import CourseContent from "./CourseContent.svelte";
  import CourseSidebar from "./CourseSidebar.svelte";
</script>

<svelte:head>
  <title>Course Details | Xavier Entrepreneurship Bootcamp</title>
</svelte:head>

<PageHeader title="Course Details" />

<img src="/courses/course-thumbnail.jpg" alt="" class="course-bg" />

<div class="course-content container">
  <CourseContent />
  <CourseSidebar />
</div>

<style>
  .course-bg {
    max-width: 1300px;
    width: 100%;
    border-radius: var(--radius-600);
    margin: 8rem auto 0 auto;
    object-fit: cover;
    height: 570px;
  }

  .course-content {
    display: grid;
    grid-template-columns: 8fr 4fr;
    margin-top: -3rem;
    gap: 3rem;
    margin-bottom: 8rem;
  }

  @media screen and (max-width: 68em) {
    .course-content {
      gap: 1rem;
      grid-template-columns: 8fr 5fr;
    }
  }

  @media screen and (max-width: 57em) {
    .course-content {
      grid-template-columns: 1fr;
      margin-top: 0;
    }

    .course-content {
      margin-bottom: 2rem;
    }

    .course-bg {
      margin-top: 0;
      border-radius: 0;
    }
  }
</style>
