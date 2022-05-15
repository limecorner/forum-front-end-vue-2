<template>
  <div class="container py-5">
    <NavTabs />

    <h1 class="mt-5">最新動態</h1>
    <hr />
    <div class="row">
      <div class="col-md-6">
        <h3>最新餐廳</h3>
        <!-- 最新餐廳 NewestRestaurants -->
        <NewestRestaurants :restaurants="restaurants" />
      </div>
      <div class="col-md-6">
        <!-- 最新評論 NewestComments-->
        <h3>最新評論</h3>
      </div>
    </div>
  </div>
</template>

<script>
import NavTabs from "../components/NavTabs.vue";
import NewestRestaurants from "../components/NewestRestaurants.vue";
const dummyData = {
  restaurants: [
    {
      id: 41,
      name: "Vince Harvey",
      tel: "549-257-3341",
      address: "22758 Ford Island",
      opening_hours: "08:00",
      description:
        "Vitae occaecati totam saepe culpa est dignissimos dolorum ducimus. Voluptas quam doloremque corporis aut qui. Quis ea laboriosam. Blanditiis quia unde eligendi et possimus expedita. Eaque facere illo eos dolore omnis enim vitae ipsa. Minus dolorem eos earum.",
      image:
        "https://loremflickr.com/320/240/restaurant,food/?random=73.16169638627655",
      viewCounts: 0,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      CategoryId: 1,
      Category: {
        id: 1,
        name: "中式料理",
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
    },
    {
      id: 34,
      name: "Shaylee Bogisich",
      tel: "625.592.8672",
      address: "48780 Jennings Roads",
      opening_hours: "08:00",
      description: "delectus facilis et",
      image:
        "https://loremflickr.com/320/240/restaurant,food/?random=73.2619399965599",
      viewCounts: 0,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      CategoryId: 2,
      Category: null,
    },
    {
      id: 32,
      name: "Major King",
      tel: "(383) 003-0966 x268",
      address: "653 Smitham Prairie",
      opening_hours: "08:00",
      description: "recusandae",
      image:
        "https://loremflickr.com/320/240/restaurant,food/?random=78.83210625519422",
      viewCounts: 0,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      CategoryId: 3,
      Category: {
        id: 3,
        name: "義大利料理",
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
    },
    {
      id: 24,
      name: "Miss Cole Gibson",
      tel: "(863) 552-4070 x3203",
      address: "0760 Monahan Cape",
      opening_hours: "08:00",
      description:
        "Quasi ullam voluptate exercitationem fugit. Fugiat nam et ut sit nihil velit qui. Reprehenderit fugiat quasi et cupiditate. Iste error ut saepe. Qui doloribus dolor architecto fugit et sit quam.\n \rQuas cupiditate commodi aut reprehenderit. Voluptatibus aut molestias maxime. Consequatur sit adipisci neque vel. Quam voluptas eius numquam odit. Vero at nobis et corrupti recusandae est labore. Perspiciatis quos consectetur.\n \rAliquid et eos voluptates voluptatem. Adipisci et totam. Ratione itaque ipsa reprehenderit corporis veniam itaque quo dicta. Nesciunt quas unde et ducimus quis recusandae sequi.",
      image:
        "https://loremflickr.com/320/240/restaurant,food/?random=73.42180592958908",
      viewCounts: 0,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      CategoryId: 4,
      Category: {
        id: 4,
        name: "墨西哥料理",
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
    },
    {
      id: 13,
      name: "Kenyon Thiel",
      tel: "1-677-694-3204 x333",
      address: "78018 Harley Pass",
      opening_hours: "08:00",
      description:
        "Quia unde odit eos. Quia ut qui provident autem ex id. Rerum consequatur esse laboriosam expedita molestiae distinctio similique sint voluptatem. Omnis id culpa.",
      image:
        "https://loremflickr.com/320/240/restaurant,food/?random=30.566696060117813",
      viewCounts: 0,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      CategoryId: 5,
      Category: {
        id: 5,
        name: "素食料理",
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
    },
    {
      id: 31,
      name: "Merl Miller",
      tel: "(354) 670-3033",
      address: "34290 Anissa Islands",
      opening_hours: "08:00",
      description:
        "Enim dolorem incidunt dolor eligendi nam dolor qui est aliquam.\nCommodi libero dicta non cupiditate ut delectus esse.\nBeatae quisquam dolores in ut expedita non ipsam nisi et.\nEveniet et laboriosam unde aut perferendis ut velit.\nMolestiae rerum rem rerum voluptas nostrum eligendi dolor aperiam doloribus.",
      image:
        "https://loremflickr.com/320/240/restaurant,food/?random=49.811122007190804",
      viewCounts: 0,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      CategoryId: 5,
      Category: {
        id: 5,
        name: "素食料理",
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
    },
    {
      id: 6,
      name: "Lew Abernathy",
      tel: "(739) 673-7188 x26411",
      address: "6801 Becker Lakes",
      opening_hours: "08:00",
      description: "Quis aut sed eos ipsa minus odio.",
      image:
        "https://loremflickr.com/320/240/restaurant,food/?random=86.87143591840167",
      viewCounts: 0,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      CategoryId: 1,
      Category: {
        id: 1,
        name: "中式料理",
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
    },
    {
      id: 46,
      name: "Gordon Hansen",
      tel: "836.891.4846 x29078",
      address: "31834 Stehr Stravenue",
      opening_hours: "08:00",
      description: "facere dolores ut",
      image:
        "https://loremflickr.com/320/240/restaurant,food/?random=70.08310217328886",
      viewCounts: 0,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      CategoryId: 1,
      Category: {
        id: 1,
        name: "中式料理",
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
    },
    {
      id: 37,
      name: "Mr. Adolph Mueller",
      tel: "1-080-338-4901",
      address: "0753 Peggie Trafficway",
      opening_hours: "08:00",
      description:
        "Vel incidunt quam quasi ut suscipit unde et. Eaque dolores ut perferendis ipsa praesentium.",
      image:
        "https://loremflickr.com/320/240/restaurant,food/?random=42.5251726473364",
      viewCounts: 0,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      CategoryId: 2,
      Category: {
        id: 2,
        name: "日本料理",
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
    },
    {
      id: 44,
      name: "Erin Von",
      tel: "1-678-118-8811",
      address: "25257 Runte Rue",
      opening_hours: "08:00",
      description: "libero",
      image:
        "https://loremflickr.com/320/240/restaurant,food/?random=71.3357759663752",
      viewCounts: 0,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      CategoryId: 3,
      Category: {
        id: 3,
        name: "義大利料理",
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
    },
  ],
  comments: [
    {
      id: 4,
      text: "Est molestiae dolores molestias.",
      UserId: 1,
      RestaurantId: 4,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      User: {
        id: 1,
        name: "root",
        email: "root@example.com",
        password:
          "$2a$10$dEj2FuoeieIlkN.GJfoC9O.SwoaY99MfXet4z8vB5wAf12Vwa5NjS",
        isAdmin: true,
        image: null,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
      Restaurant: {
        id: 4,
        name: "Joshua Weber",
        tel: "424-024-2249 x96905",
        address: "163 Edythe Freeway",
        opening_hours: "08:00",
        description: "amet",
        image:
          "https://loremflickr.com/320/240/restaurant,food/?random=6.0287430229847505",
        viewCounts: 0,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
        CategoryId: 4,
      },
    },
    {
      id: 46,
      text: "Voluptas hic enim.",
      UserId: 1,
      RestaurantId: 46,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      User: {
        id: 1,
        name: "root",
        email: "root@example.com",
        password:
          "$2a$10$dEj2FuoeieIlkN.GJfoC9O.SwoaY99MfXet4z8vB5wAf12Vwa5NjS",
        isAdmin: true,
        image: null,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
      Restaurant: {
        id: 46,
        name: "Gordon Hansen",
        tel: "836.891.4846 x29078",
        address: "31834 Stehr Stravenue",
        opening_hours: "08:00",
        description: "facere dolores ut",
        image:
          "https://loremflickr.com/320/240/restaurant,food/?random=70.08310217328886",
        viewCounts: 0,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
        CategoryId: 1,
      },
    },
    {
      id: 66,
      text: "Est fuga possimus esse.",
      UserId: 1,
      RestaurantId: 16,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      User: {
        id: 1,
        name: "root",
        email: "root@example.com",
        password:
          "$2a$10$dEj2FuoeieIlkN.GJfoC9O.SwoaY99MfXet4z8vB5wAf12Vwa5NjS",
        isAdmin: true,
        image: null,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
      Restaurant: {
        id: 16,
        name: "Ivy Kohler",
        tel: "(974) 030-3672 x1291",
        address: "7860 Vladimir Ferry",
        opening_hours: "08:00",
        description:
          "Voluptatibus rerum ad perferendis in dignissimos vitae.\nDicta nulla eaque et omnis deleniti odio reiciendis.",
        image:
          "https://loremflickr.com/320/240/restaurant,food/?random=55.07993364721075",
        viewCounts: 0,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
        CategoryId: 5,
      },
    },
    {
      id: 83,
      text: "Exercitationem deleniti ratione autem inventore facere explicabo architecto.",
      UserId: 1,
      RestaurantId: 33,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      User: {
        id: 1,
        name: "root",
        email: "root@example.com",
        password:
          "$2a$10$dEj2FuoeieIlkN.GJfoC9O.SwoaY99MfXet4z8vB5wAf12Vwa5NjS",
        isAdmin: true,
        image: null,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
      Restaurant: {
        id: 33,
        name: "Mr. Ila Runolfsson",
        tel: "1-152-236-7326",
        address: "667 Richard Harbor",
        opening_hours: "08:00",
        description: "nulla molestias quaerat",
        image:
          "https://loremflickr.com/320/240/restaurant,food/?random=28.46843426576937",
        viewCounts: 0,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
        CategoryId: 1,
      },
    },
    {
      id: 106,
      text: "Nihil minus dolor aperiam.",
      UserId: 1,
      RestaurantId: 6,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      User: {
        id: 1,
        name: "root",
        email: "root@example.com",
        password:
          "$2a$10$dEj2FuoeieIlkN.GJfoC9O.SwoaY99MfXet4z8vB5wAf12Vwa5NjS",
        isAdmin: true,
        image: null,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
      Restaurant: {
        id: 6,
        name: "Lew Abernathy",
        tel: "(739) 673-7188 x26411",
        address: "6801 Becker Lakes",
        opening_hours: "08:00",
        description: "Quis aut sed eos ipsa minus odio.",
        image:
          "https://loremflickr.com/320/240/restaurant,food/?random=86.87143591840167",
        viewCounts: 0,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
        CategoryId: 1,
      },
    },
    {
      id: 139,
      text: "Est repellat cum et recusandae odio.",
      UserId: 1,
      RestaurantId: 39,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      User: {
        id: 1,
        name: "root",
        email: "root@example.com",
        password:
          "$2a$10$dEj2FuoeieIlkN.GJfoC9O.SwoaY99MfXet4z8vB5wAf12Vwa5NjS",
        isAdmin: true,
        image: null,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
      Restaurant: {
        id: 39,
        name: "Mable Fritsch",
        tel: "887.432.7849 x56726",
        address: "0438 Reilly Green",
        opening_hours: "08:00",
        description:
          "Eius omnis deserunt labore quos. Qui quis voluptates modi voluptatem aut. Nostrum labore nisi et ipsum dolore autem repudiandae. Voluptatibus aut a. Suscipit cupiditate modi aliquam eos iure non. Quia optio est.",
        image:
          "https://loremflickr.com/320/240/restaurant,food/?random=37.94075816638185",
        viewCounts: 0,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
        CategoryId: 1,
      },
    },
    {
      id: 24,
      text: "Quidem inventore aut quisquam est rerum.",
      UserId: 2,
      RestaurantId: 24,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      User: {
        id: 2,
        name: "user1",
        email: "user1@example.com",
        password:
          "$2a$10$bX6prwanTs8SK6l/74g3UOWAbGURSxcrmvZlCjsFKBfOtz.P6nhba",
        isAdmin: false,
        image: null,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
      Restaurant: {
        id: 24,
        name: "Miss Cole Gibson",
        tel: "(863) 552-4070 x3203",
        address: "0760 Monahan Cape",
        opening_hours: "08:00",
        description:
          "Quasi ullam voluptate exercitationem fugit. Fugiat nam et ut sit nihil velit qui. Reprehenderit fugiat quasi et cupiditate. Iste error ut saepe. Qui doloribus dolor architecto fugit et sit quam.\n \rQuas cupiditate commodi aut reprehenderit. Voluptatibus aut molestias maxime. Consequatur sit adipisci neque vel. Quam voluptas eius numquam odit. Vero at nobis et corrupti recusandae est labore. Perspiciatis quos consectetur.\n \rAliquid et eos voluptates voluptatem. Adipisci et totam. Ratione itaque ipsa reprehenderit corporis veniam itaque quo dicta. Nesciunt quas unde et ducimus quis recusandae sequi.",
        image:
          "https://loremflickr.com/320/240/restaurant,food/?random=73.42180592958908",
        viewCounts: 0,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
        CategoryId: 4,
      },
    },
    {
      id: 49,
      text: "Corrupti impedit et amet ex necessitatibus amet aut minima dolores.",
      UserId: 2,
      RestaurantId: 49,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      User: {
        id: 2,
        name: "user1",
        email: "user1@example.com",
        password:
          "$2a$10$bX6prwanTs8SK6l/74g3UOWAbGURSxcrmvZlCjsFKBfOtz.P6nhba",
        isAdmin: false,
        image: null,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
      Restaurant: {
        id: 49,
        name: "Mr. Jazmyn Boehm",
        tel: "595.522.0044 x6012",
        address: "5283 Pacocha Mountain",
        opening_hours: "08:00",
        description: "Dolores id dolores.",
        image:
          "https://loremflickr.com/320/240/restaurant,food/?random=76.41242000222897",
        viewCounts: 0,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
        CategoryId: 2,
      },
    },
    {
      id: 91,
      text: "Sapiente optio omnis odit.",
      UserId: 2,
      RestaurantId: 41,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      User: {
        id: 2,
        name: "user1",
        email: "user1@example.com",
        password:
          "$2a$10$bX6prwanTs8SK6l/74g3UOWAbGURSxcrmvZlCjsFKBfOtz.P6nhba",
        isAdmin: false,
        image: null,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
      Restaurant: {
        id: 41,
        name: "Vince Harvey",
        tel: "549-257-3341",
        address: "22758 Ford Island",
        opening_hours: "08:00",
        description:
          "Vitae occaecati totam saepe culpa est dignissimos dolorum ducimus. Voluptas quam doloremque corporis aut qui. Quis ea laboriosam. Blanditiis quia unde eligendi et possimus expedita. Eaque facere illo eos dolore omnis enim vitae ipsa. Minus dolorem eos earum.",
        image:
          "https://loremflickr.com/320/240/restaurant,food/?random=73.16169638627655",
        viewCounts: 0,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
        CategoryId: 1,
      },
    },
    {
      id: 112,
      text: "Suscipit beatae debitis.",
      UserId: 2,
      RestaurantId: 12,
      createdAt: "2022-03-11T06:14:36.000Z",
      updatedAt: "2022-03-11T06:14:36.000Z",
      User: {
        id: 2,
        name: "user1",
        email: "user1@example.com",
        password:
          "$2a$10$bX6prwanTs8SK6l/74g3UOWAbGURSxcrmvZlCjsFKBfOtz.P6nhba",
        isAdmin: false,
        image: null,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
      },
      Restaurant: {
        id: 12,
        name: "Jeramy Prohaska",
        tel: "027.433.7642 x66093",
        address: "34373 Opal Place",
        opening_hours: "08:00",
        description:
          "Nostrum qui voluptas soluta provident praesentium voluptatibus nulla sed.",
        image:
          "https://loremflickr.com/320/240/restaurant,food/?random=38.70140963092747",
        viewCounts: 0,
        createdAt: "2022-03-11T06:14:36.000Z",
        updatedAt: "2022-03-11T06:14:36.000Z",
        CategoryId: 2,
      },
    },
  ],
};

export default {
  components: {
    NavTabs,
    NewestRestaurants,
  },
  data() {
    return {
      restaurants: [],
      comments: [],
    };
  },
  methods: {
    fetchRestaurants() {
      const { restaurants, comments } = dummyData;
      this.restaurants = restaurants;
      this.comments = comments;
    },
  },
  created() {
    this.fetchRestaurants();
  },
};
</script>