<template>
  <div style="background-color: #f7f7f7">
    <div
      class="text-center"
      style="
        background: linear-gradient(to right, #009933 20%, #333399 90%);
        height: 15em;
      "
    >
      <h1 class="pt-15 white--text" style="font-size: 45px">Blog</h1>
      <p style="font-weight: bold; font-size: 20px">Article Details</p>
    </div>
    <div style="background-color: #f7f7f7">
      
        <v-container>
          <h3 class="mb-16">
            Home > <span style="color: #999999">Blog Single</span>
          </h3>
          <v-card height="80em" elevation="0">
            <v-container class="pa-16">
              <h1 style="font-size: 36px">
                Finding best places to visit in California
              </h1>

              <div class="pr-16 pt-8">
                <v-row class="pr-16">
                  <v-col>
                    <h5>Date</h5>
                    <p>July 25, 2017</p>
                  </v-col>
                  <v-col>
                    <h5>Category</h5>
                    <p>Food, Breakfast</p>
                  </v-col>
                  <v-col>
                    <h5>Tag</h5>
                    <p style="width: 300px">
                      Burger, Pixxa, Drink, Hot, Spacial
                    </p>
                  </v-col>
                  <v-col>
                    <h5>View</h5>
                    <p>35</p>
                  </v-col>
                  <v-col class="pr-16">
                    <h5 class="pr-16">Like</h5>
                    <p class="pr-16">09</p>
                  </v-col>
                </v-row>
               
                  <v-img src="california.jpg"></v-img>
              
                <p  style="font-size: 17px">
                  Adipiscing elit commodo ligula eget dolor Morlem ipsum dolor
                  sit amet nec, consectetuer adipiscing elit. Aenean commod
                  ligula eget dolor Cum sociis natoque penatibus et magnis dis
                  parturient montes. Morlem ipsum dolor sit amet nec penatib et
                  magnis dis parturient montes. Morlem ipsum dolor sit amet nec,
                  consectetuer adipiscing elit. Aenean commodo ligulaits eget
                  dolor. Aenean massa. Cum sociis nato que pena tibus et magnis
                  dis par tu rient montes. Morlem ipsum dolor set amet nec,
                  consectetuer adipiscing elit. Aenean commodo ligula eget
                  dolor.
                </p>
                <p  style="font-size: 17px">
                  .Nommodo ligula eget dolor Morlem ipsum dolor sit amet nec,
                  conse ctetuer adipi-scing elit. Aenean commod ligula eget
                  dolor Cum sociis natoque penatibus et magnis dis parturient
                  montes. Morlem ipsum dolor sit amet nec penatib et magnis dis
                  parturient montes. Morlem ipstium dolor sit amet nec, conse
                  ctetuer adipiscing elit. Aenean commodo ligulaits eget is
                  dolor. Aenean massa. Cum sociis nato que pena tibus et magnis
                  dis partu rient montes. Morlem ipsum dolor set amet nec,
                  consectetuer adipiscing elit. Aenean commodo ligula eget
                  dolor.
                </p>
                <v-row>
                  <p class="mt-16" style="font-weight: bold">Share:</p>
                  <div class="mt-15">
                    <v-icon class="pl-5">mdi-facebook</v-icon>
                    <v-icon class="pl-2">mdi-instagram</v-icon>
                    <v-icon class="pl-2">mdi-twitter</v-icon>
                    <v-icon class="pl-2">mdi-heart</v-icon>
                  </div>
                </v-row>
              </div>
            </v-container>
          </v-card>
        </v-container>
        <div class="mt-16">
          <h1 class="text-center">Related Post</h1>
          <v-container>
          <blog />
          </v-container>
        </div>
        <comments />
        <reply />
      </div>
    
  </div>
</template>

<script>
import blog from "~/components/blog.vue";
import Comments from "~/components/comments.vue";
import Reply from "~/components/reply.vue";
export default {
  components: { blog, Comments, Reply },
};
</script>

<style></style>
