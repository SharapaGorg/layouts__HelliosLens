<template>
  <div>
    <center>
      <div class='mainDisplay'>
        <div class='monsterBokeh' style='top : 181px'>MONSTER BOKEH</div>
        <div class='bigText' style='top : 281px'>Legendary Helios lens</div>
        <div class='monsterBokeh' style='top : 428px'>With adapter for your camera and free worldwide shipping</div>
        <img src='../static/arrow.svg' class='arrow'/>
      </div>

      <div class='main-content'>
        <div class='examples-inscription'>Examples of photos taken on Helios</div>
        <div class='image-box'>
          <img src='../static/image1.svg' class='image1'/>
          <img src='../static/image2.svg' class='image2'/>
          <img src='../static/image3.svg' class='image3'/>
          <img src='../static/image4.svg' class='image4'/>
          <img src='../static/image5.svg' class='image5'/>
          <img src='../static/image6.svg' class='image6'/>
          <img src='../static/image7.svg' class='image7'/>
          <img src='../static/image8.svg' class='image8'/>
        </div>
        <br><br><br><br><br><br><br><br><br><br><br><br>
        <div class='examples-inscription'>Technical characteristics of Helios lens</div>

        <div class='technical-characteristics'>
          <div class='col-start-2'>
            <technical-characteristic svg-path="tech1.svg" title='Focal length 50mm-85mm'
                                      description="This focal length is great fot shooting portraits"/>
          </div>

          <div class='col-start-3'>
            <technical-characteristic svg-path="tech2.svg" title='6-13 diaphragm petals'
                                      description="In the pictures draws a remarkable blur of areas of sharpness (side)."/>
          </div>

          <div class='col-start-4'>
            <technical-characteristic title-w="96"
                                      svg-path="tech3.svg" title='Luminosil 1.5-2.0'
                                      description="Enough for shooting in moderate lighting conditions."/>
          </div>

          <div class='col-start-5'>
            <technical-characteristic svg-path="tech4.svg" title="Optical diagram of type 'Planar'"
                                      description="The optical circuit was copied from the Carl Zeiss Jena Biotar 2/58 lens."/>
          </div>
        </div>

        <div class='dandelion-box'>
          <span class='header'>More opportunities for creativity</span>
          <span class='description'>Focus, diaphragm and hold settings with manual lenses take place in manual mode "M," this gives more opportunities for creativity</span>
          <img src='../static/arrow.svg'/>
        </div>

        <span class = 'examples-inscription' style ='display: block; margin-bottom : 240px'>Buy a helios lens</span>
        <div class = 'filter-box'>
          <div class = 'filter-dropdown'>
            <img class = 'dropdownArrow' src = '../static/dropdownArrow.svg'>
            <span>Порядок: по умолчан</span>
          </div>
          <div class = 'zoom-container'>
            <img src = '../static/zoom.svg' class = 'zoom'/>
          </div>
          <input class = 'filter-text-field' placeholder = 'Поиск'>
        </div>
        <div class = 'helios'>
            <HeliosLens :img-path="heliosUnit.imgPath" :title="heliosUnit.title" :price="heliosUnit.price"/>
            <HeliosLens :img-path="heliosUnit.imgPath" :title="heliosUnit.title" :price="heliosUnit.price" />
            <HeliosLens :img-path="heliosUnit.imgPath" :title="heliosUnit.title" :price="heliosUnit.price" />
            <HeliosLens :img-path="heliosUnit.imgPath" :title="heliosUnit.title" :price="heliosUnit.price" />
            <HeliosLens :img-path="heliosUnit.imgPath" :title="heliosUnit.title" :price="heliosUnit.price" />
            <HeliosLens :img-path="heliosUnit.imgPath" :title="heliosUnit.title" :price="heliosUnit.price" />
        </div>
      </div>
    </center>
  </div>
</template>

<script>

import TechnicalCharacteristic from "../components/technicalCharacteristic";
import HeliosLens from "../components/HeliosLens";

export default {
  data() {
    return {
      heliosUnit : {
        imgPath : "helios.png",
        title : "Helios 44M-4 58mm f/2",
        price : "$45"
      }
    }
  },
  mounted() {
  },
  components: {
    TechnicalCharacteristic,
    HeliosLens
  }
}
</script>
