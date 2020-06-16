<template>
  <div class="wrap">
    <ul class="movie-list">
      <li class="item" v-for="item in movieList" :key="item.id">
        <div class="cover"><img :src="item.images.small"></div>
        <div class="detail">
          <div>{{item.title}}</div>
          <div class="info">
            <span v-for="(item, index) in item.pubdates" :key="index">{{item}} </span>/
            <span><span v-for="(item, index) in item.pubdates" :key="index">{{item}} </span>/</span>
            <!-- <span v-for="item in item.genres" :key="item">{{item}} </span>/ -->
            <span v-for="item in item.directors" :key="item.id">{{item.name}} </span>/
            <span v-for="item in item.casts" :key="item.id">{{item.name}} </span>
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {
      movieList: [
        {
          id: "27186348",
          title: "春潮",
          images: {
            large: "https://img9.doubanio.com/view/photo/s_ratio_poster/public/p2604517782.jpg",
            medium: "https://img9.doubanio.com/view/photo/s_ratio_poster/public/p2604517782.jpg",
            small: "https://img9.doubanio.com/view/photo/s_ratio_poster/public/p2604517782.jpg"
          },
          pubdates: ["2019-06-18(上海电影节)", "2020-05-17(中国大陆网络)"],
          genres: ["剧情", "家庭"],
          directors: [
            {
              alt: "https://movie.douban.com/celebrity/1301413/",
              avatars: {
                small: "https://img9.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1382599051.49.jpg", 
                large: "https://img9.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1382599051.49.jpg", 
                medium: "https://img9.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1382599051.49.jpg"
              },
              id: "1301413",
              name: "杨荔钠",
              name_en: "Lina Yang"
            }
          ],
          casts: [
            {
              alt: "https://movie.douban.com/celebrity/1042568/",
              avatars: {
                small: "https://img9.doubanio.com/view/celebrity/s_ratio_celebrity/public/p13664.jpg", 
                large: "https://img9.doubanio.com/view/celebrity/s_ratio_celebrity/public/p13664.jpg", 
                medium: "https://img9.doubanio.com/view/celebrity/s_ratio_celebrity/public/p13664.jpg"
              },
              id: "1042568",
              name: "郝蕾",
              name_en: "Lei Hao"
            },
            {
              alt: "https://movie.douban.com/celebrity/1280673/",
              avatars: {
                small: "https://img9.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1492482412.84.jpg", 
                large: "https://img9.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1492482412.84.jpg", 
                medium: "https://img9.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1492482412.84.jpg"
              },
              id: "1280673",
              name: "金燕玲",
              name_en: "Elaine Jin"
            },
            {
              alt: "https://movie.douban.com/celebrity/1372944/",
              avatars: {
                small: "https://img9.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1493556015.71.jpg", 
                large: "https://img9.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1493556015.71.jpg", 
                medium: "https://img9.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1493556015.71.jpg"
              },
              id: "1372944",
              name: "曲隽希",
              name_en: "Junxi Qu"
            }
          ]
        },
        {
          id: "33420285",
          title: "真心半解",
          images: {
            large: "https://img9.doubanio.com/view/photo/s_ratio_poster/public/p2594916975.jpg",
            medium: "https://img9.doubanio.com/view/photo/s_ratio_poster/public/p2594916975.jpg",
            small: "https://img9.doubanio.com/view/photo/s_ratio_poster/public/p2594916975.jpg"
          },
          pubdates: ["2020-05-01(美国)"],
          genres: ["喜剧", "爱情", "同性"],
          directors: [
            {
              alt: "https://movie.douban.com/celebrity/1045482/",
              avatars: {
                small: "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1495865667.03.jpg", 
                large: "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1495865667.03.jpg", 
                medium: "https://img3.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1495865667.03.jpg"
              },
              id: "1045482",
              name: "伍思薇",
              name_en: "Alice Wu"
            }
          ],
          casts: [
            {
              alt: "https://movie.douban.com/celebrity/1256835/",
              avatars: {
                small: "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1588349291.37.jpg", 
                large: "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1588349291.37.jpg", 
                medium: "https://img1.doubanio.com/view/celebrity/s_ratio_celebrity/public/p1588349291.37.jpg"
              },
              id: "1256835",
              name: "莉娅·刘易斯",
              name_en: "Leah Lewis"
            },
            {
              alt: "https://movie.douban.com/celebrity/1419076/",
              avatars: {
                small: "https://img3.doubanio.com/view/celebrity/s_ratio_c…/p_tPqdbHYV0Acel_avatar_uploaded1561530200.93.jpg", 
                large: "https://img3.doubanio.com/view/celebrity/s_ratio_c…/p_tPqdbHYV0Acel_avatar_uploaded1561530200.93.jpg", 
                medium: "https://img3.doubanio.com/view/celebrity/s_ratio_c…/p_tPqdbHYV0Acel_avatar_uploaded1561530200.93.jpg"
              },
              id: "1419076",
              name: "丹尼尔·迪默",
              name_en: "Daniel Diemer"
            },
            {
              alt: "https://movie.douban.com/celebrity/1418708/",
              avatars: {
                small: "https://img3.doubanio.com/view/celebrity/s_ratio_c…/p_tPqdbHYV0Acel_avatar_uploaded1561117508.93.jpg", 
                large: "https://img3.doubanio.com/view/celebrity/s_ratio_c…/p_tPqdbHYV0Acel_avatar_uploaded1561117508.93.jpg", 
                medium: "https://img3.doubanio.com/view/celebrity/s_ratio_c…/p_tPqdbHYV0Acel_avatar_uploaded1561117508.93.jpg"
              },
              id: "1418708",
              name: "艾丽克西斯·勒梅尔",
              name_en: "Alexxis Lemire"
            }
          ]
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
.wrap {
  width: 375px;
  height: 667px;
  margin-left: 20px;
  overflow-y: auto;
  box-shadow: 0 0 10px rgba(0,0,0,0.2);
  border-radius: 4px;
}
.movie-list {
  padding: 10px;
  .item {
    display: flex;
    padding: 10px 0;
    .cover {
      width: 50px;
      img {
        width: 100%;
        vertical-align: middle;
        border-radius: 4px;
      }
    }
    .detail {
      flex: 1;
      margin-left: 10px;
      .title {
        color: #333;
        font-size: 16px;
        font-weight: bold;
      }
      .info {
        display: -webkit-box;
        -webkit-line-clamp: 2;
        -webkit-box-orient: vertical;
        overflow: hidden;

        color: #888;
        font-size: 12px;
      }
    }
  }
}
</style>