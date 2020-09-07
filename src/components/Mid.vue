<template>
  <div class="middle-container">
    <img src="../assets/pictures/pic2.jpg" />
    <div>
      <button>
        <p>Kopiera koden</p>
        <p>spot on 2020</p>
        <p>till urklipp</p>
      </button>
      <button>Maila bokning</button>
    </div>
    <h2>Andra förmåner</h2>
  </div>
</template>

<script>
export default {
  name: "Mid",
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
.middle-container {
  display: flex;
  flex-direction: column;
  align-items: center;

  h2 {
    margin: 50px 50px 80px 50px;
  }

  img {
    width: 1280px;
    height: 550px;
    object-fit: cover;
  }

  div {
    display: flex;
    flex-direction: row;
    justify-content: center;
    width: 100%;

    button {
      border-style: none;
      padding-top: 15px;
      padding-bottom: 15px;
      margin: 40px 40px 40px 0px;
      color: color(white_);
      border-radius: 2px;
      box-shadow: 1px 4px 8px color(shadow_);
    }
    button:hover {
      cursor: pointer;
      opacity: 0.8;
    }

    button:nth-child(2) {
      width: 128px;
      background-color: color(black_);
    }
    button:nth-child(1) {
      display: flex;
      flex-direction: row;
      justify-content: center;
      width: 448px;
      background-color: color(red_);

      p {
        padding: 0px 0px 0px 0px;
        margin-right: 3px;
        text-transform: uppercase;
        font-weight: bold;
      }

      p:nth-child(2) {
        text-decoration: underline;
      }
    }
  }
}
</style>
