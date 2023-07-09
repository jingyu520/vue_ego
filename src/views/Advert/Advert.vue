<template>
  <div class="ad-category">
    <div
      v-for="(category, index) in categories"
      :key="index"
      class="ad-category__item"
    >
      <h3 class="ad-category__title">{{ category.name }}</h3>
      <ul class="ad-list">
        <li
          v-for="(ad, index) in category.ads"
          :key="index"
          class="ad-list__item"
        >
          <a :href="ad.link" class="ad-link">{{ ad.title }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>


<script>
export default {
  data() {
    return {
      categories: [
        {
          name: "生活服务",
          ads: [
            { title: "洗衣服务", link: "#" },
            { title: "便利店", link: "#" },
            { title: "快递服务", link: "#" },
          ],
        },
        {
          name: "教育培训",
          ads: [
            { title: "小学辅导", link: "#" },
            { title: "英语培训", link: "#" },
            { title: "IT培训", link: "#" },
          ],
        },
        {
          name: "餐饮美食",
          ads: [
            { title: "火锅", link: "#" },
            { title: "西餐", link: "#" },
            { title: "烧烤", link: "#" },
          ],
        },
        {
          name: "生活服务",
          ads: [
            { title: "洗衣服务", link: "#" },
            { title: "便利店", link: "#" },
            { title: "快递服务", link: "#" },
          ],
        },
        {
          name: "餐饮美食",
          ads: [
            { title: "火锅", link: "#" },
            { title: "西餐", link: "#" },
            { title: "烧烤", link: "#" },
          ],
        },
        {
          name: "教育培训",
          ads: [
            { title: "小学辅导", link: "#" },
            { title: "英语培训", link: "#" },
            { title: "IT培训", link: "#" },
          ],
        },
        {
          name: "餐饮美食",
          ads: [
            { title: "火锅", link: "#" },
            { title: "西餐", link: "#" },
            { title: "烧烤", link: "#" },
          ],
        },
        {
          name: "生活服务",
          ads: [
            { title: "洗衣服务", link: "#" },
            { title: "便利店", link: "#" },
            { title: "快递服务", link: "#" },
          ],
        },
      ],
    };
  },
};
</script>

<style scoped>
.ad-category {
  display: flex;
  flex-wrap: wrap;
  margin: 10px;
}

.ad-category__item {
  /* 33.333% */
  width: calc(30.7% - 20px);
  margin: 10px;
  padding: 16px;
  border: 1px solid #ccc;
  border-radius: 4px;
  background-color: #fff;
  box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.1);
}

.ad-category__title {
  font-size: 20px;
  font-weight: bold;
  margin-top: 0;
  margin-bottom: 16px;
}

.ad-list {
  list-style: none;
  margin: 0;
  padding: 0;
}

.ad-list__item {
  margin-top: 12px;
  font-size: 16px;
  line-height: 1.5;
}

.ad-link {
  color: #0066cc;
  text-decoration: none;
}

.ad-link:hover {
  color: #00447e;
  text-decoration: underline;
}
</style>