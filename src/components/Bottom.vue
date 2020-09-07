<template>
  <div class="bottom-container">
    <ul>
      <li v-bind:key="li.id" v-for="li in bookingList">
        <div>
          <button>
            <svg
              xmlns="http://www.w3.org/2000/svg"
              x="0px"
              y="0px"
              width="24"
              height="24"
              viewBox="0 0 172 172"
              style=" fill:#000000;"
            >
              <g
                fill="none"
                fill-rule="nonzero"
                stroke="none"
                stroke-width="1"
                stroke-linecap="butt"
                stroke-linejoin="miter"
                stroke-miterlimit="10"
                stroke-dasharray
                stroke-dashoffset="0"
                font-family="none"
                font-weight="none"
                font-size="none"
                text-anchor="none"
                style="mix-blend-mode: normal"
              >
                <path d="M0,172v-172h172v172z" fill="none" />
                <g fill="#f1f1f1">
                  <path
                    d="M123.56901,42.94401c-2.18814,0.00053 -4.1576,1.32735 -4.98006,3.35504c-0.82245,2.0277 -0.33375,4.35156 1.23575,5.87624l26.65804,26.65804h-133.94108c-1.93842,-0.02741 -3.74144,0.99102 -4.71865,2.66532c-0.97721,1.6743 -0.97721,3.74507 0,5.41937c0.97721,1.6743 2.78023,2.69273 4.71865,2.66532h133.94108l-26.65804,26.65804c-1.40412,1.34815 -1.96971,3.35005 -1.47866,5.23364c0.49105,1.88359 1.96202,3.35456 3.84561,3.84561c1.88359,0.49105 3.88549,-0.07455 5.23364,-1.47866l35.83333,-35.83333c2.09823,-2.0991 2.09823,-5.50149 0,-7.60059l-35.83333,-35.83333c-1.01222,-1.0424 -2.4033,-1.63064 -3.85628,-1.6307z"
                  />
                </g>
              </g>
            </svg>
          </button>
          <p class="category">{{li.cat}}</p>
          <img :src="li.pic" />
          <div>
            <h3>{{li.title}}</h3>
            <div class="location">
              <svg
                xmlns="http://www.w3.org/2000/svg"
                x="0px"
                y="0px"
                width="24"
                height="24"
                viewBox="0 0 172 172"
                style=" fill:#000000;"
              >
                <g
                  fill="none"
                  fill-rule="nonzero"
                  stroke="none"
                  stroke-width="1"
                  stroke-linecap="butt"
                  stroke-linejoin="miter"
                  stroke-miterlimit="10"
                  stroke-dasharray
                  stroke-dashoffset="0"
                  font-family="none"
                  font-weight="none"
                  font-size="none"
                  text-anchor="none"
                  style="mix-blend-mode: normal"
                >
                  <path d="M0,172v-172h172v172z" fill="none" />
                  <g fill="#ac4842">
                    <path
                      d="M86,14.33333c-27.70633,0 -50.16667,22.46033 -50.16667,50.16667c0,35.83333 50.16667,93.16667 50.16667,93.16667c0,0 50.16667,-57.33333 50.16667,-93.16667c0,-27.70633 -22.46033,-50.16667 -50.16667,-50.16667zM86,82.41667c-9.89717,0 -17.91667,-8.0195 -17.91667,-17.91667c0,-9.89717 8.0195,-17.91667 17.91667,-17.91667c9.89717,0 17.91667,8.0195 17.91667,17.91667c0,9.89717 -8.0195,17.91667 -17.91667,17.91667z"
                    />
                  </g>
                </g>
              </svg>
              <p>{{li.pos}}</p>
            </div>
            <p class="card-text">{{li.text}}</p>
          </div>
        </div>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "HelloWorld",
  data() {
    return {
      bookingList: [
        {
          id: "1",
          title: "Fantastisk mat på fina fat",
          text: "Spara 25% på din nästa bokning",
          cat: "Mat & Dryck",
          pos: "Linköping",
          pic: require("../assets/pictures/pic4.jpg"),
        },
        {
          id: "2",
          title: "Fantastisk mat på fina fat",
          text: "Spara 25% på din nästa bokning",
          cat: "Mat & Dryck",
          pos: "Malmö",
          pic: require("../assets/pictures/pic7.jpg"),
        },
        {
          id: "3",
          title: "Fantastisk mat på fina fat",
          text: "Spara 25% på din nästa bokning",
          cat: "Mat & Dryck",
          pos: "Stockholm",
          pic: require("../assets/pictures/pic6.jpg"),
        },
        {
          id: "4",
          title: "Vandra höga kusten",
          text: "Guide från 695 kr/dagen",
          cat: "Sport & Fritid",
          pos: "Härnösand",
          pic: require("../assets/pictures/pic8.jpg"),
        },
        {
          id: "5",
          title: "Drömhotell med takterass",
          text: "Spara 25% på din nästa bokning",
          cat: "Hotell & Boende",
          pos: "Göteborg",
          pic: require("../assets/pictures/pic3.jpg"),
        },
        {
          id: "6",
          title: "Boka konferens",
          text: "Spara 25% på din nästa bokning",
          cat: "Hotell & Boende",
          pos: "Stockholm",
          pic: require("../assets/pictures/pic5.jpg"),
        },
        {
          id: "7",
          title: "Cykla höga kusten",
          text: "Guide från 695 kr/dagen",
          cat: "Sport & Fritid",
          pos: "Härnösand",
          pic: require("../assets/pictures/pic9.jpg"),
        },
        {
          id: "8",
          title: "Fantastisk mat på fina fat",
          text: "Spara 25% på din nästa bokning",
          cat: "Mat & Dryck",
          pos: "Stockholm",
          pic: require("../assets/pictures/pic6.jpg"),
        },
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
$colors: (
  white_: #ffffff,
  background_: #f3f2ed,
  red_: #ac4842,
  black_: #000,
  gray_: #f1f1f1,
  hoverBlack_: rgb(26, 26, 26),
  shadow_: rgb(151, 151, 151),
);

@function color($color-name) {
  @return map-get($colors, $color-name);
}
.bottom-container {
  padding-bottom: 60px;
  ul {
    display: grid;
    grid-template-columns: 260px 260px 260px 260px;
    column-gap: 40px;
    row-gap: 40px;
    align-items: center;
    justify-content: center;
  }

  li {
    list-style: none;
  }

  h3 {
    padding: 12px;
    font-weight: bolder;
  }

  .card-text {
    padding: 12px 12px 18px 12px;
  }

  div {
    width: 260px;
    background-color: color(white_);

    button {
      z-index: 100;
      position: absolute;
      border-style: none;
      background-color: color(black_);
      border-radius: 2px;
      box-shadow: 1px 4px 8px color(shadow_);
      padding: 10px;
      margin: 127px 0px 0px 225px;
    }
    button:hover {
      cursor: pointer;
      background-color: color(hoverBlack_);
    }
    img {
      width: 260px;
      height: 150px;
      object-fit: cover;
      border-bottom: 4px solid color(red_);
    }
    .category {
      z-index: 100;
      position: absolute;
      font-size: 13px;
      background-color: color(background_);
      color: color(black_);
      font-weight: bold;
      margin: 10px 0px 0px 15px;
      padding: 4px;
      border-radius: 2px;
    }
    .location {
      display: flex;
      flex-direction: row;
      margin: 4px 0px 4px 0px;
      padding-left: 6px;
      p {
        text-transform: uppercase;
        font-size: 14px;
        font-weight: bold;
        color: color(red_);
        margin-top: 4px;
      }
    }
  }
}
</style>
