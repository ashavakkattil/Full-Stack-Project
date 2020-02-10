<template>
  <v-container>
    <v-card v-for="(blog,index) in blogs" :key="index" height="200" class="mb-5 blogPostList">
      <v-row>
        <v-col cols="4">
          <v-img :src="blog.src" aspect-ratio="16/9" height="180px" />
        </v-col>
        <v-col cols="8"></v-col>
      </v-row>
    </v-card>
  </v-container>
</template>
<script>
export default {
  data() {
    return {
      blogs: [
        {
          name: "Rose, Coffee & Life",
          desc: "Rose, Coffee & Life blog post 1",
          category: "Personal",
          src:
            "https://www.designlabthemes.com/preview/type/files/2017/07/cake-1839134_1920-800x500.jpg"
        },
        {
          name: "LifeStyle Blog & Shop",
          desc: "LifeStyle Blog & Shop blog post 2",
          category: "Personal",
          src:
            "https://www.designlabthemes.com/preview/type/files/2017/07/cake-1839134_1920-800x500.jpg"
        },
        {
          name: "Diy Holiday",
          desc: "Diy Holiday blog post 3",
          category: "Health",
          src:
            "https://www.designlabthemes.com/preview/type/files/2017/07/mobile-791164-800x500.jpg"
        },
        {
          name: "Behind the Lens",
          desc: "Behind the Lens blog post 4",
          category: "Food",
          src:
            "https://www.designlabthemes.com/preview/type/files/2017/07/cake-1839134_1920-800x500.jpg"
        },
        {
          name: "Why flower Succeeds",
          desc: "Why flower Succeeds blog post 5",
          category: "Work",
          src:
            "https://www.designlabthemes.com/preview/type/files/2017/07/mobile-791164-800x500.jpg"
        },
        {
          name: "Some random thoughts",
          desc: "Some random thoughts post 6",
          category: "Personal",
          src:
            "https://www.designlabthemes.com/preview/type/files/2017/07/cake-1839134_1920-800x500.jpg"
        }
      ]
    };
  }
};
</script>
<style scoped>
.blogPostList .col {
  display: inline-flex;
}
</style>