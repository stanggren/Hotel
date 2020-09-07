<template>
  <div class="top-container">
    <div class="left-container">
      <div>
        <p class="top-cat">Mat & Dryck</p>
        <button class="gallery-btn left">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            x="0px"
            y="0px"
            width="24"
            height="24"
            viewBox="0 0 172 172"
            style=" fill:#ffffff;"
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
              <g fill="#ffffff">
                <path
                  d="M123.56901,42.94401c-2.18814,0.00053 -4.1576,1.32735 -4.98006,3.35504c-0.82245,2.0277 -0.33375,4.35156 1.23575,5.87624l26.65804,26.65804h-133.94108c-1.93842,-0.02741 -3.74144,0.99102 -4.71865,2.66532c-0.97721,1.6743 -0.97721,3.74507 0,5.41937c0.97721,1.6743 2.78023,2.69273 4.71865,2.66532h133.94108l-26.65804,26.65804c-1.40412,1.34815 -1.96971,3.35005 -1.47866,5.23364c0.49105,1.88359 1.96202,3.35456 3.84561,3.84561c1.88359,0.49105 3.88549,-0.07455 5.23364,-1.47866l35.83333,-35.83333c2.09823,-2.0991 2.09823,-5.50149 0,-7.60059l-35.83333,-35.83333c-1.01222,-1.0424 -2.4033,-1.63064 -3.85628,-1.6307z"
                />
              </g>
            </g>
          </svg>
        </button>
        <button class="gallery-btn right">
          <svg
            xmlns="http://www.w3.org/2000/svg"
            x="0px"
            y="0px"
            width="24"
            height="24"
            viewBox="0 0 172 172"
            style=" fill:#ffffff;"
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
              <g fill="#ffffff">
                <path
                  d="M123.56901,42.94401c-2.18814,0.00053 -4.1576,1.32735 -4.98006,3.35504c-0.82245,2.0277 -0.33375,4.35156 1.23575,5.87624l26.65804,26.65804h-133.94108c-1.93842,-0.02741 -3.74144,0.99102 -4.71865,2.66532c-0.97721,1.6743 -0.97721,3.74507 0,5.41937c0.97721,1.6743 2.78023,2.69273 4.71865,2.66532h133.94108l-26.65804,26.65804c-1.40412,1.34815 -1.96971,3.35005 -1.47866,5.23364c0.49105,1.88359 1.96202,3.35456 3.84561,3.84561c1.88359,0.49105 3.88549,-0.07455 5.23364,-1.47866l35.83333,-35.83333c2.09823,-2.0991 2.09823,-5.50149 0,-7.60059l-35.83333,-35.83333c-1.01222,-1.0424 -2.4033,-1.63064 -3.85628,-1.6307z"
                />
              </g>
            </g>
          </svg>
        </button>
        <img src="../assets/pictures/pic1.jpg" />
      </div>
      <div>
        <div>
          <h2>Om</h2>
          <ul>
            <li>Gäller för två personer i ett dubbelrum standard med frukost.</li>
            <li>Tillägg för tredje person i extrabädd 200kr inkl frukost.</li>
            <li>Gäller förhandsbokning av en natt fredag till lördag eller lördag till söndag fram till och med 27 juni 2020.</li>
          </ul>
        </div>
        <div id="overlay">
          <h2>Så utnyttjar du förmånen</h2>
          <ul>
            <li>Boka på telefon 013-25 26 00 eller mejla till q.ekoxen@choice.se</li>
            <li>Uppge bokningskod Mera ekoxen 2020 för att få MERA-pris</li>
          </ul>
        </div>
      </div>
    </div>
    <div class="right-container">
      <div>
        <h1>Bo på Hotel Ekoxen i Linköping</h1>
        <span></span>
        <p>Bo på Quality Hotel Ekoxen med vackert läge i Linköping. Granne med stadens gröna oas Trädgårdsföreningen och bara ett stenkast från centrums alla restauranger, butiker och kulturinrättningar.</p>
        <p id="price">895 kr/natt</p>
        <div>
          <button>Maila bokning</button>
          <button>
            <p>Kopiera koden</p>
            <p>spot on 2020</p>
            <p>till urklipp</p>
          </button>
        </div>
      </div>
      <div>
        <p>Quality Hotel Ekoxen</p>
        <img src="../assets/pictures/map.png" />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Top",
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

.top-container {
  .gallery-btn {
    border-style: none;
    padding: 20px;
    border-radius: 2px;
    box-shadow: 0px 3px 6px rgb(110, 110, 110);
    z-index: 100;
    position: absolute;
    background-color: color(black_);
  }

  .gallery-btn:hover {
    cursor: pointer;
    background-color: color(hoverBlack_);
  }

  .left {
    margin: 305px 0px 0px 481px;
    svg {
      transform: rotate(180deg);
    }
  }
  .right {
    margin: 305px 0px 0px 546px;
  }
  .top-cat {
    z-index: 100;
    position: absolute;
    font-size: 13px;
    background-color: color(background_);
    color: color(red_);
    font-weight: bold;
    margin: 15px 0px 0px 540px;
    padding: 4px;
    border-radius: 2px;
  }

  display: flex;
  flex-direction: row;
  justify-content: center;

  .left-container {
    display: flex;
    flex-direction: column;

    div:nth-child(1) {
      img {
        width: 100%;
      }
    }

    div:nth-child(2) {
      #overlay {
        z-index: 100;
        position: absolute;
      }

      h2 {
        padding-bottom: 10px;
      }

      li {
        margin: 20px 20px 20px 20px;
      }

      div:nth-child(1) {
        background-color: color(white_);
        width: 490px;
        padding: 20px;
        margin-top: 40px;
        margin-left: 120px;
      }
      div:nth-child(2) {
        background-color: color(white_);
        width: 490px;
        padding: 20px;
        margin-top: 30px;
        margin-left: 120px;
        padding-bottom: 25px;
      }
    }
  }

  .right-container {
    display: flex;
    flex-direction: column;
    justify-content: center;

    div:nth-child(1) {
      width: 640px;
      height: 460px;
      background-color: color(white_);
      h1 {
        padding: 40px 100px 10px 100px;
        font-size: 40px;
        text-align: center;
        font-weight: 500;
      }
      span {
        display: block;
        border-style: solid;
        border-width: 4px;
        color: color(red_);
        width: 200px;
        margin-left: auto;
        margin-right: auto;
        margin-bottom: 20px;
        border-radius: 2px;
      }
      p {
        text-align: center;
        padding: 0px 100px 10px 100px;
      }

      #price {
        color: color(red_);
        font-size: 25px;
        margin-top: 10px;
      }

      div {
        display: flex;
        flex-direction: column;
        align-items: center;

        button {
          border-style: none;
          padding-top: 15px;
          padding-bottom: 15px;
          color: color(white_);
          border-radius: 2px;
          box-shadow: 1px 4px 8px color(shadow_);
        }
        button:hover {
          cursor: pointer;
          opacity: 0.8;
        }

        button:nth-child(1) {
          width: 20%;
          margin-top: 30px;
          background-color: color(black_);
        }
        button:nth-child(2) {
          display: flex;
          flex-direction: row;
          justify-content: center;
          width: 70%;
          background-color: color(red_);
          margin-top: 20px;

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
    div:nth-child(2) {
      margin-top: 20px;
      margin-bottom: 20px;
      margin-left: 20px;
      border: solid 8px color(white_);
      width: 466px;
      height: 336px;

      p {
        background-color: color(background_);
        padding: 10px;
        font-size: 14px;
        font-weight: bold;
      }
      img {
        width: 450px;
      }
    }
  }
}
</style>
