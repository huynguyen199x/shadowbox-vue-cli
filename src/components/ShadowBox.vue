<template>
  <div id="main">
    <div class="Polaris-Page">
      <div class="Polaris-Page__Content">
        <div class="Polaris-Layout">
          <div class="Polaris-Layout__Section Polaris-Layout__Section--oneHalf">
            <div class="Polaris-Card">
              <div class="Polaris-Card__Header">
                <h2 class="Polaris-Heading">Box-Shadow CSS Generator</h2>
              </div>
              <div class="Polaris-Card__Section">
                <div class="Polaris-FormLayout">
                  <div class="Polaris-FormLayout__Item">
                    <div class="">
                      <div class="Polaris-Labelled__LabelWrapper">
                        <div class="Polaris-Label">
                          <label
                            id="PolarisRangeSlider1Label"
                            for="PolarisRangeSlider1"
                            class="Polaris-Label__Text"
                            >Shift right</label
                          >
                        </div>
                      </div>
                      <div
                        class="Polaris-RangeSlider-SingleThumb"
                        :style="shiftRightStyle"
                      >
                        <div
                          class="Polaris-RangeSlider-SingleThumb__InputWrapper"
                        >
                          <input
                            v-model.number="shiftRight"
                            type="range"
                            class="Polaris-RangeSlider-SingleThumb__Input"
                            id="PolarisRangeSlider1"
                            name="PolarisRangeSlider1"
                            min="-50"
                            max="50"
                            step="1"
                            aria-valuemin="-50"
                            aria-valuemax="50"
                            :aria-valuenow="shiftRight"
                            aria-invalid="false"
                          /><output
                            for="PolarisRangeSlider1"
                            class="Polaris-RangeSlider-SingleThumb__Output"
                          >
                            <div
                              class="
                                Polaris-RangeSlider-SingleThumb__OutputBubble
                              "
                            >
                              <span
                                class="
                                  Polaris-RangeSlider-SingleThumb__OutputText
                                "
                                >{{ shiftRight }}</span
                              >
                            </div>
                          </output>
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="Polaris-FormLayout__Item">
                    <div class="">
                      <div class="Polaris-Labelled__LabelWrapper">
                        <div class="Polaris-Label">
                          <label
                            id="PolarisRangeSlider2Label"
                            for="PolarisRangeSlider2"
                            class="Polaris-Label__Text"
                            >Shift down</label
                          >
                        </div>
                      </div>
                      <div
                        class="Polaris-RangeSlider-SingleThumb"
                        :style="shiftDownStyle"
                      >
                        <div
                          class="Polaris-RangeSlider-SingleThumb__InputWrapper"
                        >
                          <input
                            v-model.number="shiftDown"
                            type="range"
                            class="Polaris-RangeSlider-SingleThumb__Input"
                            id="PolarisRangeSlider2"
                            name="PolarisRangeSlider2"
                            min="-50"
                            max="50"
                            step="1"
                            value="-21"
                            aria-valuemin="-50"
                            aria-valuemax="50"
                            aria-valuenow="-21"
                            aria-invalid="false"
                          /><output
                            for="PolarisRangeSlider2"
                            class="Polaris-RangeSlider-SingleThumb__Output"
                          >
                            <div
                              class="
                                Polaris-RangeSlider-SingleThumb__OutputBubble
                              "
                            >
                              <span
                                class="
                                  Polaris-RangeSlider-SingleThumb__OutputText
                                "
                                >{{ shiftDown }}</span
                              >
                            </div>
                          </output>
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="Polaris-FormLayout__Item">
                    <div class="">
                      <div class="Polaris-Labelled__LabelWrapper">
                        <div class="Polaris-Label">
                          <label
                            id="PolarisRangeSlider3Label"
                            for="PolarisRangeSlider3"
                            class="Polaris-Label__Text"
                            >Spread</label
                          >
                        </div>
                      </div>
                      <div
                        class="Polaris-RangeSlider-SingleThumb"
                        :style="spreadBarStyle"
                      >
                        <div
                          class="Polaris-RangeSlider-SingleThumb__InputWrapper"
                        >
                          <input
                            v-model.number="spread"
                            type="range"
                            class="Polaris-RangeSlider-SingleThumb__Input"
                            id="PolarisRangeSlider3"
                            name="PolarisRangeSlider3"
                            min="0"
                            max="100"
                            step="1"
                            value="30"
                            aria-valuemin="0"
                            aria-valuemax="100"
                            aria-valuenow="30"
                            aria-invalid="false"
                          /><output
                            for="PolarisRangeSlider3"
                            class="Polaris-RangeSlider-SingleThumb__Output"
                          >
                            <div
                              class="
                                Polaris-RangeSlider-SingleThumb__OutputBubble
                              "
                            >
                              <span
                                class="
                                  Polaris-RangeSlider-SingleThumb__OutputText
                                "
                                >{{ spread }}</span
                              >
                            </div>
                          </output>
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="Polaris-FormLayout__Item">
                    <div class="">
                      <div class="Polaris-Labelled__LabelWrapper">
                        <div class="Polaris-Label">
                          <label
                            id="PolarisRangeSlider4Label"
                            for="PolarisRangeSlider4"
                            class="Polaris-Label__Text"
                            >Blur</label
                          >
                        </div>
                      </div>
                      <div
                        class="Polaris-RangeSlider-SingleThumb"
                        :style="blurBarStyle"
                      >
                        <div
                          class="Polaris-RangeSlider-SingleThumb__InputWrapper"
                        >
                          <input
                            v-model.number="blur"
                            type="range"
                            class="Polaris-RangeSlider-SingleThumb__Input"
                            id="PolarisRangeSlider4"
                            name="PolarisRangeSlider4"
                            min="0"
                            max="100"
                            step="1"
                            value="5"
                            aria-valuemin="0"
                            aria-valuemax="100"
                            aria-valuenow="5"
                            aria-invalid="false"
                          /><output
                            for="PolarisRangeSlider4"
                            class="Polaris-RangeSlider-SingleThumb__Output"
                          >
                            <div
                              class="
                                Polaris-RangeSlider-SingleThumb__OutputBubble
                              "
                            >
                              <span
                                class="
                                  Polaris-RangeSlider-SingleThumb__OutputText
                                "
                                >{{ blur }}</span
                              >
                            </div>
                          </output>
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="Polaris-FormLayout__Item">
                    <div class="">
                      <div class="Polaris-Labelled__LabelWrapper">
                        <div class="Polaris-Label">
                          <label
                            id="PolarisRangeSlider5Label"
                            for="PolarisRangeSlider5"
                            class="Polaris-Label__Text"
                            >Opacity</label
                          >
                        </div>
                      </div>
                      <div
                        class="Polaris-RangeSlider-SingleThumb"
                        :style="opacityBarStyle"
                      >
                        <div
                          class="Polaris-RangeSlider-SingleThumb__InputWrapper"
                        >
                          <input
                            v-model.number="opacity"
                            type="range"
                            class="Polaris-RangeSlider-SingleThumb__Input"
                            id="PolarisRangeSlider5"
                            name="PolarisRangeSlider5"
                            min="0"
                            max="100"
                            step="1"
                            value="10"
                            aria-valuemin="0"
                            aria-valuemax="100"
                            aria-valuenow="10"
                            aria-invalid="false"
                          /><output
                            for="PolarisRangeSlider5"
                            class="Polaris-RangeSlider-SingleThumb__Output"
                          >
                            <div
                              class="
                                Polaris-RangeSlider-SingleThumb__OutputBubble
                              "
                            >
                              <span
                                class="
                                  Polaris-RangeSlider-SingleThumb__OutputText
                                "
                                >{{ opacity }}</span
                              >
                            </div>
                          </output>
                        </div>
                      </div>
                    </div>
                  </div>
                  <div class="Polaris-FormLayout__Item">
                    <label class="Polaris-Choice" for="PolarisCheckbox1"
                      ><span class="Polaris-Choice__Control"
                        ><span class="Polaris-Checkbox"
                          ><input
                            v-model="inset"
                            type="checkbox"
                            id="PolarisCheckbox1"
                            class="Polaris-Checkbox__Input"
                            aria-invalid="false"
                            role="checkbox"
                            aria-checked="false"
                            value="" /><span
                            class="Polaris-Checkbox__Backdrop"
                          ></span
                          ><span class="Polaris-Checkbox__Icon"
                            ><span class="Polaris-Icon"
                              ><svg
                                viewBox="0 0 20 20"
                                class="Polaris-Icon__Svg"
                                focusable="false"
                                aria-hidden="true"
                              >
                                <path
                                  d="M8.315 13.859l-3.182-3.417a.506.506 0 0 1 0-.684l.643-.683a.437.437 0 0 1 .642 0l2.22 2.393 4.942-5.327a.437.437 0 0 1 .643 0l.643.684a.504.504 0 0 1 0 .683l-5.91 6.35a.437.437 0 0 1-.642 0"
                                ></path></svg></span></span></span></span
                      ><span class="Polaris-Choice__Label">Inset</span></label
                    >
                  </div>
                  <div class="Polaris-FormLayout__Item">
                    <div>
                      <input
                        v-model="shadowColor"
                        type="color"
                        id="favcolor"
                        name="favcolor"
                      />
                    </div>
                  </div>
                </div>
              </div>
              <div class="Polaris-Card__Section">
                <button
                  type="button"
                  class="Polaris-Button"
                  @click="addLayerHandler"
                >
                  <span class="Polaris-Button__Content"
                    ><span class="Polaris-Button__Text">Add Layer</span></span
                  ></button
                ><br /><br />

                
                  <ul class="layer_wrap__1hYkm">
                    <div>
                    <draggable :list="layers" :sort="true">
                      <li
                        v-for="(layer, index) in layersCss"
                        :key="index"
                        :class="
                          index == currentLayer
                            ? currentLayerClass
                            : layerLayerClass
                        "
                        @click="setCurrentLayer(index)"
                        data-id="0"
                      >
                        <span class="layer_drag__2AEZM"
                          ><span class="Polaris-Icon"
                            ><svg
                              viewBox="0 0 20 20"
                              class="Polaris-Icon__Svg"
                              focusable="false"
                              aria-hidden="true"
                            >
                              <path
                                d="M7 2a2 2 0 1 0 .001 4.001A2 2 0 0 0 7 2m0 6a2 2 0 1 0 .001 4.001A2 2 0 0 0 7 8m0 6a2 2 0 1 0 .001 4.001A2 2 0 0 0 7 14m6-8a2 2 0 1 0-.001-4.001A2 2 0 0 0 13 6m0 2a2 2 0 1 0 .001 4.001A2 2 0 0 0 13 8m0 6a2 2 0 1 0 .001 4.001A2 2 0 0 0 13 14"
                              ></path></svg></span></span
                        >{{ layer
                        }}<span class="layer_edit__u4bnF"
                          ><span class="Polaris-Icon"
                            ><svg
                              viewBox="0 0 20 20"
                              class="Polaris-Icon__Svg"
                              focusable="false"
                              aria-hidden="true"
                            >
                              <path
                                d="M17.086 2.912a3.126 3.126 0 0 0-4.414 0l-9.379 9.379a.998.998 0 0 0-.263.464l-1 4a1 1 0 0 0 1.212 1.213l4-1c.176-.044.337-.135.465-.263l9.38-9.379a3.125 3.125 0 0 0 0-4.414zm-1.414 3L15 6.584l-1.586-1.586.672-.672a1.125 1.125 0 0 1 1.586 0 1.123 1.123 0 0 1 0 1.586zM5.414 12.998L12 6.412l1.586 1.586L7 14.584l-1.586-1.586z"
                                fill-rule="evenodd"
                              ></path></svg></span></span
                        ><span
                          @click="delLayerHandler(index)"
                          class="layer_del__QYHb8"
                          ><span class="Polaris-Icon"
                            ><svg
                              viewBox="0 0 20 20"
                              class="Polaris-Icon__Svg"
                              focusable="false"
                              aria-hidden="true"
                            >
                              <path
                                d="M16 6H4a1 1 0 1 0 0 2h1v9a1 1 0 0 0 1 1h8a1 1 0 0 0 1-1V8h1a1 1 0 1 0 0-2zM9 4a1 1 0 1 1 0-2h2a1 1 0 1 1 0 2H9zm2 12h2V8h-2v8zm-4 0h2V8H7v8z"
                                fill-rule="evenodd"
                              ></path></svg></span
                        ></span>
                      </li>
                    </draggable>
                    </div>
                  </ul>
              </div>
            </div>
          </div>
          <div class="Polaris-Layout__Section Polaris-Layout__Section--oneHalf">
            <div class="jsx-4089688463 jsx-117178027 Polaris-Card">
              <div class="jsx-4089688463 jsx-117178027 Polaris-Card__Header">
                <h2 class="jsx-4089688463 jsx-117178027 Polaris-Heading">
                  Preview
                </h2>
                <div
                  class="
                    jsx-4089688463 jsx-117178027
                    preview_colorpicker__2nfvL
                  "
                >
                  <div>
                    <input
                      v-model="previewBoxBackgroundColor"
                      type="color"
                      id="favcolor"
                      name="favcolor"
                    />
                  </div>
                  <div>
                    <input
                      v-model="boxColor"
                      type="color"
                      id="favcolor"
                      name="favcolor"
                    />
                  </div>
                </div>
              </div>
              <div
                class="
                  jsx-4089688463 jsx-117178027
                  Polaris-Card__Section
                  previewarea
                "
                :style="{ 'background-color': previewBoxBackgroundColor }"
              >
                <div
                  style="width: 200px; height: 200px"
                  class="react-resizable"
                >
                  <div
                    class="preview-box"
                    :style="{
                      'box-shadow': shadowLayersCss,
                      'background-color': boxColor,
                    }"
                  ></div>
                  <span
                    class="react-resizable-handle react-resizable-handle-se"
                    style="touch-action: none"
                  ></span>
                </div>
              </div>
            </div>
            <div class="Polaris-Card">
              <div class="Polaris-Card__Header">
                <h2 class="Polaris-Heading">CSS code</h2>
              </div>
              <div class="Polaris-Card__Section">
                <pre><code>{{cssCode}}</code></pre>
              </div>
            </div>
            <div class="Polaris-Card">
              <div class="Polaris-Card__Header">
                <h2 class="Polaris-Heading">Template</h2>
              </div>
              <div class="Polaris-Card__Section">
                <div class="template">
                  <div class="template__global template__1"></div>
                  <div class="template__global template__2"></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import draggable from "vuedraggable";
export default {
  name: "ShadowBox",
  components: {
    draggable,
  },
  data() {
    return {
      currentLayerClass: "layer_current__1y7nK",
      layerLayerClass: "layer_layer__1L3ov",
      shiftRight: 0,
      shiftDown: 0,
      spread: 0,
      blur: 0,
      opacity: 0,
      inset: false,
      layers: [],
      currentLayer: 0,
      boxColor: "#3D9DF6",
      shadowColor: "#000000",
      previewBoxBackgroundColor: "#ffffff",
    };
  },
  mounted() {
    this.layers.push(this.shadowValue);
  },
  computed: {
    layersCss() {
      return this.layers.map((layer) => {
        var inset = layer[5] ? " inset" : "";
        return `rgba(${this.hexToRgba(layer[0][0], layer[0][1] / 100)}) ${
          layer[1]
        }px ${layer[2]}px ${layer[3]}px ${layer[4]}px${inset}`;
      });
    },
    
    cssCode() {
      return `box-shadow: ${this.shadowLayersCss};`;
    },

    shadowLayersCss() {
      return `${this.layersCss.join(",")}`;
    },
    shadowRbgaColor() {
      return [this.shadowColor, this.opacity];
    },

    shadowValue() {
      return [
        this.shadowRbgaColor,
        this.shiftRight,
        this.shiftDown,
        this.blur,
        this.spread,
        this.inset,
      ];
    },

    shiftRightStyle() {
      return this.rangeSliderStyle(-50, 50, this.shiftRight);
    },

    shiftDownStyle() {
      return this.rangeSliderStyle(-50, 50, this.shiftDown);
    },

    spreadBarStyle() {
      return this.rangeSliderStyle(0, 100, this.spread);
    },

    opacityBarStyle() {
      return this.rangeSliderStyle(0, 100, this.opacity);
    },

    blurBarStyle() {
      return this.rangeSliderStyle(0, 100, this.blur);
    },
  },

  methods: {
    setShadowValue(shadowValue) {
      this.shadowColor = shadowValue[0][0];
      this.opacity = shadowValue[0][1];
      this.shiftRight = shadowValue[1];
      this.shiftDown = shadowValue[2];
      this.blur = shadowValue[3];
      this.spread = shadowValue[4];
      this.inset = shadowValue[5];
    },

    rangeSliderStyle(min, max, current) {
      var outputFactor = ((50 - (current - min)) / 100).toFixed(1);
      return `--Polaris-RangeSlider-min:${min}; --Polaris-RangeSlider-max:${max}; --Polaris-RangeSlider-current:${current}; --Polaris-RangeSlider-progress:${
        current - min
      }%; --Polaris-RangeSlider-output-factor:${outputFactor};`;
    },

    addLayerHandler() {
      this.layers.push(["#000000", 0, 5, 3, 0.2, false]);
    },

    setCurrentLayer(index) {
      this.currentLayer = index;
      this.setShadowValue(this.layers[index]);
    },

    delLayerHandler(index) {
      if (this.layers.length == 1) return;
      this.layers.splice(index, 1);
    },

    hexToRgba(hex, opacity) {
      var bigint = parseInt(hex.slice(1), 16);
      var r = (bigint >> 16) & 255;
      var g = (bigint >> 8) & 255;
      var b = bigint & 255;
      return r + "," + g + "," + b + "," + opacity;
    },
  },

  watch: {
    shadowValue() {
      this.$set(this.layers, this.currentLayer, this.shadowValue);
    },
  },
};
</script>

<style>
#main {
  --top-bar-background: #00848e;
  --top-bar-background-lighter: #1d9ba4;
  --top-bar-color: #f9fafb;
  --p-frame-offset: 0px;
}
</style>