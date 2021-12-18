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

        <span class='examples-inscription' style='display: block; margin-bottom : 240px'>Buy a helios lens</span>
        <div class='filter-box'>
          <div class='filter-dropdown'>
            <img class='dropdownArrow' src='../static/dropdownArrow.svg'>
            <span>Порядок: по умолчан</span>
          </div>
          <div class='zoom-container'>
            <img src='../static/zoom.svg' class='zoom'/>
          </div>
          <input class='filter-text-field' placeholder='Поиск'>
        </div>
        <div class='helios'>
          <HeliosLens :img-path="heliosUnit.imgPath" :title="heliosUnit.title" :price="heliosUnit.price"/>
          <HeliosLens :img-path="heliosUnit.imgPath" :title="heliosUnit.title" :price="heliosUnit.price"/>
          <HeliosLens :img-path="heliosUnit.imgPath" :title="heliosUnit.title" :price="heliosUnit.price"/>
          <HeliosLens :img-path="heliosUnit.imgPath" :title="heliosUnit.title" :price="heliosUnit.price"/>
          <HeliosLens :img-path="heliosUnit.imgPath" :title="heliosUnit.title" :price="heliosUnit.price"/>
          <HeliosLens :img-path="heliosUnit.imgPath" :title="heliosUnit.title" :price="heliosUnit.price"/>
        </div>
        <button class='view-other-lenses'>
          <span>View other lenses</span>
        </button>
        <span class='examples-inscription' style='display : block; top : 0;'>History and features of Helios Lens</span>

        <div class='text-block'>
          <span class='title'>These lenses are much cheaper than modern lenses</span>
          <span class='content'>Today, many photographers are interested in old Soviet optics, and Helios lenses are no exception. Some people have been working with digital cameras with old optics for over a year. There are many reasons for this, but the main one is the low price. Lenses released in the USSR are much cheaper than modern lenses.</span>
        </div>
        <div class='text-block' style = 'margin-bottom : 60px'>
          <span class='title'>Good study of tonal transitions</span>
          <span class='content'>In addition to affordable value, old Soviet optics has a number of other undeniable advantages. Plasticity, volume and good study of tonal transitions are the main differences of the design created on Soviet lenses.</span>
        </div>
        <div class='text-block1'>
          <span class='text-content'>
            Now manufacturers of new optics try to increase sharpness and eliminate all possible image errors. Because of this, images are most often too sharp and contrasting. This is not the best ability of the lens, for example, when shooting portraits.
          </span>
        </div>
        <div class='text-block'>
          <span class='title'>Perfect for creating quality portraits</span>
          <span class='content'>The Helios optics mentioned above has its own unusual, artistic image, perfect for creating quality portraits. Modern photographic equipment has a complex optical design and sometimes more than a few dozen lenses. If you add more lenses, it will result in air loss at the borders. Often even a special multi-lighting coating will not save them. Soviet fixed lenses are made according to a simple optical scheme. They have only three or seven lenses, which is a great advantage for portrait shooting.</span>
        </div>
        <div class='text-block'>
          <span class='title'>Strength and reliability</span>
          <span class='content'>Another advantage of old optics is the strength and reliability of the metal structure and the use of only real glasses. Thanks to this, even after actively working with lenses from 1950-1960, they will still be in perfect condition.</span>
        </div>
        <div class='text-block'>
          <span class='title'>Best suited for portraits</span>
          <span class='content'>Helios 44-2 58 mm f/2.0 is a soft-focus optics that is best suited for portraits. Due to this, the frames become soft and light, minor defects are hidden, and the skin is smoothed. Helios 44-2 was produced from 1950 to 1990. It came complete with Zenit-ET and Zenit-10 cameras and, despite this, had pretty good optical characteristics.</span>
        </div>
        <div class='text-block'>
          <span class='title'>You can control the diaphragm manually</span>
          <span class = 'content'>Helios 44-2 has single-layer enlightenment and an optical circuit that consists of six parts in four groups. You can control the diaphragm manually. The threaded connection of this lens is M42. Thanks to the 58 mm focal length, the result is not very contrasting, light frames with a pleasant, slightly twisted background blur. With an open f/2.0 diaphragm and contrasting lighting, you can create a background with a side effect that will not divert attention from the main object.</span>
        </div>
        <div class='text-block'>
          <span class='title'>Before selling, all optics are specially trained and checked for damage</span>
          <span class = 'content'>Our dedicated online store offers you to buy a low-cost Helios 44-2 lens and an adapter designed specifically for your camera. Before selling, all optics posted on our site pages are specially trained and checked for damage so you can be sure of the quality of the item being purchased. If you have any questions, please contact our managers. We're always happy to help!</span>
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
      heliosUnit: {
        imgPath: "helios.png",
        title: "Helios 44M-4 58mm f/2",
        price: "$45"
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
