<template>
  <v-container>
    <v-row class="searchBoxRow">
      <v-col class="pa-0">
        <p class="subtitle font-weight-bold">Search box</p>
        <v-text-field single-line label="Search posts" outlined dense append-icon="mdi-magnify"></v-text-field>
      </v-col>
    </v-row>
    <v-row class="searchBoxRow">
      <v-col class="pa-0">
        <p class="subtitle font-weight-bold">Recent Posts</p>
        <div v-for="(blog,index) in blogs" :key="index" class="recentPost">
          <ul>
            <li>{{blog.name}}</li>
          </ul>
        </div>
      </v-col>
    </v-row>
    <v-row class="searchBoxRow">
      <v-col class="pa-0">
        <p class="subtitle font-weight-bold">Categories</p>
        <div v-for="(blog,index) in blogs" :key="index" class="recentPost">
          <ul>
            <li>{{blog.category}}(count of posts)</li>
          </ul>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<style scoped>
.searchBoxRow {
  margin-top: 30px;
}
.searchBoxRow .col {
  text-align: center;
}
.searchBoxRow p {
  text-transform: uppercase;
  padding: 10px;
  border: 1px solid yellowgreen;
}
.recentPost ul {
  list-style: none;
  text-align: justify;
  padding: 6px;
  border-bottom: 1px solid #eeeeee;
}
</style>

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