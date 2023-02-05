<template>

  <div class="text-center m-5">
    <input type="file" ref="fileInput" id="file-input" @change="handleFileUpload"/>
  </div>

  <div class="row mx-5">
    <div class="col"><div id="table-container"></div></div>
    <div class="col">

    <div class="row ms-5">
      <div class="col ">
        <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="101" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[0].kapasite}} kişi kapasiteli {{ classArray[0].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="102" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[1].kapasite}} kişi kapasiteli {{ classArray[1].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="103" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[2].kapasite}} kişi kapasiteli {{ classArray[2].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="104" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[3].kapasite}} kişi kapasiteli {{ classArray[3].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="105" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[4].kapasite}} kişi kapasiteli {{ classArray[4].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="106" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[5].kapasite}} kişi kapasiteli {{ classArray[5].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="107" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[6].kapasite}} kişi kapasiteli {{ classArray[6].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="108" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[7].kapasite}} kişi kapasiteli {{ classArray[7].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="109" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[8].kapasite}} kişi kapasiteli {{ classArray[8].sinif }} nolu sınıf
        </label>
      </div>
      </div>
      <div class="col">
        <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="201" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[9].kapasite}} kişi kapasiteli {{ classArray[9].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="202" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[10].kapasite}} kişi kapasiteli {{ classArray[10].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="203" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[11].kapasite}} kişi kapasiteli {{ classArray[11].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="204" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[12].kapasite}} kişi kapasiteli {{ classArray[12].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="205" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[13].kapasite}} kişi kapasiteli {{ classArray[13].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="206" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[14].kapasite}} kişi kapasiteli {{ classArray[14].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="207" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[15].kapasite}} kişi kapasiteli {{ classArray[15].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="208" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[16].kapasite}} kişi kapasiteli {{ classArray[16].sinif }} nolu sınıf
        </label>
      </div>
      <div class="form-check m-3">
        <input class="form-check-input" v-model="selectedOptions" type="checkbox" value="209" id="flexCheckDefault">
        <label class="form-check-label" for="flexCheckDefault">
          {{classArray[17].kapasite}} kişi kapasiteli {{ classArray[17].sinif }} nolu sınıf
        </label>
      </div>
      </div>
    </div>

    <div class="row">
      <div class="col-2"></div>
      <div class="col">
        <button @click="isSelected" :class="{'btn btn-danger p-2 mt-4': isDanger, 'btn btn-success p-2 mt-4': isSuccess}" > Öğrencileri seçili sınıflara rastgele yerleştir</button>
      </div>
      <div class="col">
        <button @click="exportToExcel" class="p-2 mt-4 btn btn-primary">Excel'e Aktar</button>
      </div>
      
    </div>

    </div>
  </div>
<!--
  <div class="row">

    
    <div class="col">
      <div>
        <ul>
          <li v-for="item in ogrenciler" :key="item.SN">
            {{item.SN}}- {{ item.ogrenciNo }} -  {{ item.ogrenciAdi}}
          </li>
        </ul>
      </div>
    </div>
    <div class="col">
      <div>
        <ul>
          <li v-for="item in shuffledList" :key="item.SN">
            {{item.SN}}- {{ item.ogrenciNo }} -  {{ item.ogrenciAdi}}
          </li>
        </ul>
      </div>
    </div>
  </div>
-->
  <div class="text-center mt-5">
    <input type="text" v-model="studentNo" placeholder="Öğrenci numarası giriniz">
    <button class="btn btn-success" @click="searchStudent">Sorgula</button>
  </div>

  <div class="text-center mt-3">
    <button class="btn btn-danger" @click="yakaKartiCikar">Yaka Kartını İndir</button>
  </div>


  <div class="container my-5" id="capture" style="width: 720px; height: 220px; border: 3px solid darkblue;">
    <div class="row">
      <div class="col-3 p-5">
        <img src=".//assets/Kırklareli_Üniversitesi_logosu.jpg" width="120" height="120">
      </div>
      <div class="col p-3 ms-4">
        <p class="fw-bold">Kırklareli Üniversitesi</p>
        <p class="fw-bold" v-if="student.info">Öğrenci Numarası: {{student.info.ogrenciNo}}</p>
        <p class="fw-bold" v-if="student.info">Öğrenci Adı ve Soyadı:{{student.info.ogrenciAdi}}</p>
        <p class="fw-bold" v-if="student.info">Dersin Adı: İleri Web Programlama</p>
        <p class="fw-bold" v-if="student.info">Sınav Tarihi: 13.01.2023 10:00</p>
      </div>
    </div>
    
  </div>

</template>

<script>
  import * as XLSX from "xlsx";
  import _ from "lodash";
  import firebase from 'firebase/compat/app';
  import 'firebase/compat/database';
  
  import 'bootstrap/dist/css/bootstrap.css';
  import 'bootstrap/dist/js/bootstrap.js';

  import html2canvas from 'html2canvas'

  let myObjStr = [];
  

 
  

export default {
  data() {
    return {
      isDanger: true,
      isSuccess: false,
      buttonText: 'Danger',
      data: [],
      items:[],
      firebaseList:[],
      shuffledList: [],
      selectedOptions: [],
      sinif_101: [],
      sinif_102: [],
      sinif_103: [],
      sinif_104: [],
      sinif_105: [],
      sinif_106: [],
      sinif_107: [],
      sinif_108: [],
      sinif_109: [],
      sinif_201: [],
      sinif_202: [],
      sinif_203: [],
      sinif_204: [],
      sinif_205: [],
      sinif_206: [],
      sinif_207: [],
      sinif_208: [],
      sinif_209: [],
      studentNo: '',
      student: {},
      classArray: [
  {
    "sinif": 101,
    "kapasite": 38
  },
  {
    "sinif": 102,
    "kapasite": 40
  },
  {
    "sinif": 103,
    "kapasite": 34
  },
  {
    "sinif": 104,
    "kapasite": 30
  },
  {
    "sinif": 105,
    "kapasite": 40
  },
  {
    "sinif": 106,
    "kapasite": 24
  },
  {
    "sinif": 107,
    "kapasite": 24
  },
  {
    "sinif": 108,
    "kapasite": 30
  },
  {
    "sinif": 109,
    "kapasite": 34
  },
  {
    "sinif": 201,
    "kapasite": 38
  },
  {
    "sinif": 202,
    "kapasite": 40
  },
  {
    "sinif": 203,
    "kapasite": 34
  },
  {
    "sinif": 204,
    "kapasite": 20
  },
  {
    "sinif": 205,
    "kapasite": 20
  },
  {
    "sinif": 206,
    "kapasite": 50
  },
  {
    "sinif": 207,
    "kapasite": 44
  },
  {
    "sinif": 208,
    "kapasite": 22
  },
  {
    "sinif": 209,
    "kapasite": 20
  }
],
      ogrenciler:[{"SN":"1","ogrenciNo":"1160505011","ogrenciAdi":" MERT KABAKÇI",},{"SN":"2","ogrenciNo":"1160505042","ogrenciAdi":" İBRAHİM KELEŞ",},{"SN":"3","ogrenciNo":"1170505002","ogrenciAdi":" HAVVA NERGİZ",},{"SN":"4","ogrenciNo":"1170505018","ogrenciAdi":" YASİN ÖZMEN",},{"SN":"5","ogrenciNo":"1170505052","ogrenciAdi":" OĞUZHAN UĞUR"},{"SN":"6","ogrenciNo":"1170505054","ogrenciAdi":" BATUHAN BERK KARADERE"},{"SN":"7","ogrenciNo":"1170505603","ogrenciAdi":" MUHAMMAD GAJENDRA ADHIRAJASA"},{"SN":"8","ogrenciNo":"1180505002","ogrenciAdi":" BERAT BİRGİN"},{"SN":"9","ogrenciNo":"1180505020","ogrenciAdi":" ECE DALPOLAT"},{"SN":"10","ogrenciNo":"1180505022","ogrenciAdi":" MUSTAFA VEYSEL KANDIRA"},{"SN":"11","ogrenciNo":"1180505025","ogrenciAdi":" MUSTAFA BİLAL VAROL"},{"SN":"12","ogrenciNo":"1180505037","ogrenciAdi":" CİHAN CİHAT GÜNHAN"},{"SN":"13","ogrenciNo":"1180505038","ogrenciAdi":" UMUT BERKAY KARACA"},{"SN":"14","ogrenciNo":"1180505045","ogrenciAdi":" EGE POLAT"},{"SN":"15","ogrenciNo":"1180505048","ogrenciAdi":" ZEYNEP AVKAROĞLU"},{"SN":"16","ogrenciNo":"1180505620","ogrenciAdi":" KÜBRA SELÇUK"},{"SN":"17","ogrenciNo":"1180505624","ogrenciAdi":" FANNISA  FIRDAUS"},{"SN":"18","ogrenciNo":"1180505801","ogrenciAdi":" İBRAHİM BURAK YAKAR"},{"SN":"19","ogrenciNo":"1180505803","ogrenciAdi":" FURKAN ASLAN"},{"SN":"20","ogrenciNo":"1180505902","ogrenciAdi":" İBRAHİM İNAL"},{"SN":"21","ogrenciNo":"1180505903","ogrenciAdi":" EDANUR HAMURCU"},{"SN":"22","ogrenciNo":"1190505001","ogrenciAdi":" ECENUR ÖZKAN"},{"SN":"23","ogrenciNo":"1190505003","ogrenciAdi":" BEYZANUR ÇETİN"},{"SN":"24","ogrenciNo":"1190505004","ogrenciAdi":" ORHAN AKARSU"},{"SN":"25","ogrenciNo":"1190505005","ogrenciAdi":" HATİCE ZEHRA ORHAN"},{"SN":"26","ogrenciNo":"1190505006","ogrenciAdi":" ERVA NUR SULTAN YALÇIN"},{"SN":"27","ogrenciNo":"1190505007","ogrenciAdi":" ERAY ALTUN"},{"SN":"28","ogrenciNo":"1190505008","ogrenciAdi":" TİMUR DÜŞÜNÜKLÜ"},{"SN":"29","ogrenciNo":"1190505010","ogrenciAdi":" HATİCE TEKİN"},{"SN":"30","ogrenciNo":"1190505011","ogrenciAdi":" FURKAN EMİRCAN DURSUN"},{"SN":"31","ogrenciNo":"1190505012","ogrenciAdi":" AHMET ŞİŞMAN"},{"SN":"32","ogrenciNo":"1190505014","ogrenciAdi":" ALAETTİN USLU"},{"SN":"33","ogrenciNo":"1190505015","ogrenciAdi":" RAHİM TÜRKMEN"},{"SN":"34","ogrenciNo":"1190505016","ogrenciAdi":" EMİR GAZİ KOPAR"},{"SN":"35","ogrenciNo":"1190505018","ogrenciAdi":" BERKE KARAALİ"},{"SN":"36","ogrenciNo":"1190505019","ogrenciAdi":" MELİKE SAĞIR"},{"SN":"37","ogrenciNo":"1190505021","ogrenciAdi":" METİN BİRİKİM KARAÇAY"},{"SN":"38","ogrenciNo":"1190505022","ogrenciAdi":" UMUT ÇAKMAK"},{"SN":"39","ogrenciNo":"1190505023","ogrenciAdi":" FURKAN KABAK"},{"SN":"40","ogrenciNo":"1190505024","ogrenciAdi":" EMİRCAN AKIN"},{"SN":"41","ogrenciNo":"1190505025","ogrenciAdi":" ÇAĞLA ÖZAY"},{"SN":"42","ogrenciNo":"1190505026","ogrenciAdi":" TUANNA BURÇAK YAVUZ"},{"SN":"43","ogrenciNo":"1190505027","ogrenciAdi":" MUSTAFA UÇAR"},{"SN":"44","ogrenciNo":"1190505028","ogrenciAdi":" ENSAR YASİN KARAKÖSE"},{"SN":"45","ogrenciNo":"1190505029","ogrenciAdi":" MUSA GÜNEY"},{"SN":"46","ogrenciNo":"1190505030","ogrenciAdi":" MUHAMMED CEYLAN"},{"SN":"47","ogrenciNo":"1190505031","ogrenciAdi":" BARIŞ ÇINAR"},{"SN":"48","ogrenciNo":"1190505032","ogrenciAdi":" HAYDAR ALÇİN"},{"SN":"49","ogrenciNo":"1190505033","ogrenciAdi":" ÖMER FARUK ERCİVAN"},{"SN":"50","ogrenciNo":"1190505035","ogrenciAdi":" ÜMMÜGÜLSÜM ALTINTAŞ"},{"SN":"51","ogrenciNo":"1190505036","ogrenciAdi":" KADİR ŞAHİN"},{"SN":"52","ogrenciNo":"1190505037","ogrenciAdi":" AHMET TURAN KARAKUŞ"},{"SN":"53","ogrenciNo":"1190505038","ogrenciAdi":" SERGEN AYTUĞ CAN"},{"SN":"54","ogrenciNo":"1190505040","ogrenciAdi":" HATTAP EMRE TANIŞ"},{"SN":"55","ogrenciNo":"1190505041","ogrenciAdi":" ÖMER FARUK TAŞ"},{"SN":"56","ogrenciNo":"1190505044","ogrenciAdi":" TAYYAR BERK ÇOBANOĞLU"},{"SN":"57","ogrenciNo":"1190505045","ogrenciAdi":" FURKAN HALİL ER"},{"SN":"58","ogrenciNo":"1190505046","ogrenciAdi":" MUSTAFA AKSAK"},{"SN":"59","ogrenciNo":"1190505048","ogrenciAdi":" AHMETCAN ÇETİN"},{"SN":"60","ogrenciNo":"1190505049","ogrenciAdi":" BAŞAK ŞİMŞEK"},{"SN":"61","ogrenciNo":"1190505050","ogrenciAdi":" MERT EROĞLU"},{"SN":"62","ogrenciNo":"1190505051","ogrenciAdi":" AHMET ENES YILDIRIM"},{"SN":"63","ogrenciNo":"1190505052","ogrenciAdi":" BATUHAN KÜÇÜKARSLAN"},{"SN":"64","ogrenciNo":"1190505054","ogrenciAdi":" DEVRİM FURKAN GÜNER"},{"SN":"65","ogrenciNo":"1190505055","ogrenciAdi":" BERK TAHA DEMİR"},{"SN":"66","ogrenciNo":"1190505056","ogrenciAdi":" ENES AY"},{"SN":"67","ogrenciNo":"1190505058","ogrenciAdi":" İBRAHİM SERHAT DEMİRCİOĞLU"},{"SN":"68","ogrenciNo":"1190505060","ogrenciAdi":" AMİNE HATUN ERGİN"},{"SN":"69","ogrenciNo":"1190505061","ogrenciAdi":" ALİ KAAN YAYLA"},{"SN":"70","ogrenciNo":"1190505062","ogrenciAdi":" ALİCAN BEKMEZ"},{"SN":"71","ogrenciNo":"1190505066","ogrenciAdi":" SİNAN TANRIKUT"},{"SN":"72","ogrenciNo":"1190505068","ogrenciAdi":" DOĞA NUR KARTAL"},{"SN":"73","ogrenciNo":"1190505069","ogrenciAdi":" ZEHRA AKGÜL"},{"SN":"74","ogrenciNo":"1190505070","ogrenciAdi":" İSMAİL KOÇ"},{"SN":"75","ogrenciNo":"1190505071","ogrenciAdi":" MUHAMMET ÜNVEREN"},{"SN":"76","ogrenciNo":"1190505072","ogrenciAdi":" SİMGE TERZİOĞLU"},{"SN":"77","ogrenciNo":"1190505624","ogrenciAdi":" DUYGU BAHAR"},{"SN":"78","ogrenciNo":"1190505804","ogrenciAdi":" BARIŞ ÜSTÜN"},{"SN":"79","ogrenciNo":"1190505902","ogrenciAdi":" MERT AVCI"},{"SN":"80","ogrenciNo":"1190505903","ogrenciAdi":" EMRAH ÇELİK"},{"SN":"81","ogrenciNo":"1200505001","ogrenciAdi":" ÖMER FARUK CENİK"},{"SN":"82","ogrenciNo":"1200505901","ogrenciAdi":" ABDUSSAMET MUHAMMED TOPAL"},{"SN":"83","ogrenciNo":"1200505904","ogrenciAdi":" YUNUS EMRE SARIDOĞAN"},{"SN":"84","ogrenciNo":"5190505044","ogrenciAdi":" AYLİN IŞIK"},{"SN":"85","ogrenciNo":"5190505046","ogrenciAdi":" ECE GÜNEŞ"},{"SN":"86","ogrenciNo":"5190505047","ogrenciAdi":" CANER KENANOĞLU"},{"SN":"87","ogrenciNo":"5190505050","ogrenciAdi":" SERHAT YILDIZ"},{"SN":"88","ogrenciNo":"5190505086","ogrenciAdi":" TİMUR ÖZTÜRK"}],
    }
  },
  mounted() {
    this.shuffleList();
    let config = {
      apiKey: "AIzaSyAGNAZ8mpO153Kp-dMfyY9prj43Pn05pVY",
      authDomain: "vue-project-d7f82.firebaseapp.com",
      databaseURL: "https://vue-project-d7f82-default-rtdb.firebaseio.com",
      projectId: "vue-project-d7f82",
      storageBucket: "vue-project-d7f82.appspot.com",
      messagingSenderId: "463132879459",
      appId: "1:463132879459:web:c69e65f53aac716920a656",
      measurementId: "G-5SKEGG1TYW"
    };
    firebase.initializeApp(config);
    let db = firebase.database();
    

    itemRef.on('value', function(snapshot) {
   
    let html = '<table>';

// Tablo başlıklarını ekleme
html += '<tr>';
for (const key in classList[0]) {
html += '<th>' + key + '</th>';
}
html += '</tr>';

// Verileri ekleme
for (const data of classList) {
html += '<tr>';
for (const key in data) {
    html += '<td>' + data[key] + '</td>';
}
html += '</tr>';
}

html += '</table>';

// Oluşturulan HTML'i sayfaya ekleme


const div = document.getElementById('table-container2');
div.innerHTML = html;
});

  },
  created() {
    
  },
  methods: {
    
    handleFileUpload(sheetName) {
      let input = this.$refs.fileInput
      let file = input.files[0]
      var extension = file.name.split('.').pop();
      if(extension !== 'xls') {
          alert('Lütfen bir excel dosyası seçiniz.');
        } else {
          
      let reader = new FileReader()
      reader.onload = (e) => {
        var data = new Uint8Array(e.target.result)
        let workbook = XLSX.read(data, { type: 'array' });

        workbook.SheetNames.forEach(function(sheetName) {
          // Here is your object
          var XL_row_object = XLSX.utils.sheet_to_row_object_array(workbook.Sheets[sheetName]);
          var json_object = JSON.stringify(XL_row_object);
          myObjStr = JSON.parse(json_object);
          let html = '<table>';

          // Tablo başlıklarını ekleme
          html += '<tr>';
          for (const key in myObjStr[0]) {
          html += '<th>' + key + '</th>';
          }
          html += '</tr>';

          // Verileri ekleme
          for (const data of myObjStr) {
          html += '<tr>';
          for (const key in data) {
              html += '<td>' + data[key] + '</td>';
          }
          html += '</tr>';
          }

          html += '</table>';

          // Oluşturulan HTML'i sayfaya ekleme


          const div = document.getElementById('table-container');
          div.innerHTML = html;
        })
      };
        /* işlemlerinizi burada yapabilirsiniz*/
        reader.readAsArrayBuffer(file)
        }

      },
      shuffleList() {
      this.shuffledList = _.shuffle(this.ogrenciler)
      console.log(this.shuffledList)
      for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    },
    async submitSelectedItems() {
      /*
      try {
        
        await firebase.database().ref('items').set(this.shuffledList)
        console.log('Successfully submitted to firebase')
      } catch (error) {
        console.log(error)
      }
      */
    },
    exportToExcel() {

      if(this.selectedOptions.includes("101")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_101);
      let wb = XLSX.utils.book_new();
      XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_101.xls")
      }
      if(this.selectedOptions.includes("102")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_102);
      let wb = XLSX.utils.book_new();
      XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_102.xls")
      }
      if(this.selectedOptions.includes("103")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_103);
      let wb = XLSX.utils.book_new();
      XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_103.xls")
      }
      if(this.selectedOptions.includes("104")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_104);
      let wb = XLSX.utils.book_new();
      XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_104.xls")
      }
      if(this.selectedOptions.includes("105")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_105);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_105.xls")
      }
      if(this.selectedOptions.includes("106")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_106);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_106.xls")
      }
      if(this.selectedOptions.includes("107")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_107);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_107.xls")
      }
      if(this.selectedOptions.includes("108")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_108);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_108.xls")
      }
      if(this.selectedOptions.includes("109")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_109);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_109.xls")
      }

      if(this.selectedOptions.includes("201")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_201);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_201.xls")
      }
      if(this.selectedOptions.includes("202")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_202);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_202.xls")
      }
      if(this.selectedOptions.includes("203")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_203);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_203.xls")
      }
      if(this.selectedOptions.includes("204")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_204);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_204.xls")
      }
      if(this.selectedOptions.includes("205")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_205);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_205.xls")
      }
      if(this.selectedOptions.includes("206")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_206);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_206.xls")
      }
      if(this.selectedOptions.includes("207")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_207);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_207.xls")
      }
      if(this.selectedOptions.includes("208")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_208);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_208.xls")
      }
      if(this.selectedOptions.includes("209")){
        let ws = XLSX.utils.json_to_sheet(this.sinif_209);
        let wb = XLSX.utils.book_new();
        XLSX.utils.book_append_sheet(wb, ws, "SheetJS");
        XLSX.writeFile(wb, "sinif_listesi_209.xls")
      }
      
    },
    async isSelected(){

      this.isDanger = !this.isDanger;
      this.isSuccess = !this.isSuccess;
      this.buttonText = this.isDanger ? 'Danger' : 'Success';

      let dbRef = firebase.database().ref("items")
      dbRef.remove()
      
      let newArray = [];
      
    
      if(this.selectedOptions.includes("101")){
        newArray = this.shuffledList.splice(0, 38);
        await firebase.database().ref('items/101').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
          this.shuffledList[i].SN = i+1;
        }
        this.sinif_101 = newArray;
      }
      if(this.selectedOptions.includes("102")){
        newArray = this.shuffledList.splice(0, 40);
        await firebase.database().ref('items/102').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
          this.shuffledList[i].SN = i+1;
        }
        this.sinif_102 = newArray;
      }
      if(this.selectedOptions.includes("103")){
        newArray = this.shuffledList.splice(0, 39);
        await firebase.database().ref('items/103').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
      }
      this.sinif_103 = newArray;
      }
      if(this.selectedOptions.includes("104")){
        newArray = this.shuffledList.splice(0, 30);
        await firebase.database().ref('items/104').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_104 = newArray;
      }
      if(this.selectedOptions.includes("105")){
        newArray = this.shuffledList.splice(0, 40);
        await firebase.database().ref('items/105').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_105 = newArray;
      }
      if(this.selectedOptions.includes("106")){
        newArray = this.shuffledList.splice(0, 24);
        await firebase.database().ref('items/106').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_106 = newArray;
      }
      if(this.selectedOptions.includes("107")){
        newArray = this.shuffledList.splice(0, 24);
        await firebase.database().ref('items/107').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_107 = newArray;
      }
      if(this.selectedOptions.includes("108")){
        newArray = this.shuffledList.splice(0, 30);
        await firebase.database().ref('items/108').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_108 = newArray;
      }
      if(this.selectedOptions.includes("109")){
        newArray = this.shuffledList.splice(0, 34);
        await firebase.database().ref('items/109').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_109 = newArray;
      }

      if(this.selectedOptions.includes("201")){
        newArray = this.shuffledList.splice(0, 38);
        await firebase.database().ref('items/201').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_201 = newArray;
      }
      if(this.selectedOptions.includes("202")){
        newArray = this.shuffledList.splice(0, 40);
        await firebase.database().ref('items/202').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_202 = newArray;
      }
      if(this.selectedOptions.includes("203")){
        newArray = this.shuffledList.splice(0, 34);
        await firebase.database().ref('items/203').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_203 = newArray;
      }
      if(this.selectedOptions.includes("204")){
        newArray = this.shuffledList.splice(0, 20);
        await firebase.database().ref('items/204').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_204 = newArray;
      }
      if(this.selectedOptions.includes("205")){
        newArray = this.shuffledList.splice(0, 20);
        await firebase.database().ref('items/205').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_205 = newArray;
      }
      if(this.selectedOptions.includes("206")){
        newArray = this.shuffledList.splice(0, 50);
        await firebase.database().ref('items/206').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_206 = newArray;
      }
      if(this.selectedOptions.includes("207")){
        newArray = this.shuffledList.splice(0, 44);
        await firebase.database().ref('items/207').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_207 = newArray;
      }
      if(this.selectedOptions.includes("208")){
        newArray = this.shuffledList.splice(0, 22);
        await firebase.database().ref('items/208').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_208 = newArray;
      }
      if(this.selectedOptions.includes("209")){
        newArray = this.shuffledList.splice(0, 20);
        await firebase.database().ref('items/209').set(newArray)
        for (let i = 0; i < this.shuffledList.length; i++) {
      this.shuffledList[i].SN = i+1;
    }
    this.sinif_209 = newArray;
      }

    },
    searchStudent() {
    var parentKey = "Student not found";
    firebase.database().ref('items').once('value', snapshot => {
        snapshot.forEach(childSnapshot => {
            childSnapshot.forEach(grandChildSnapshot => {
                if (grandChildSnapshot.val().ogrenciNo === this.studentNo) {
                    parentKey = childSnapshot.key;
                    this.student = {
                        "parentKey": parentKey,
                        "info": grandChildSnapshot.val()
                    }
                }
            });
        });
    });
  },
  yakaKartiCikar(){
    html2canvas(document.querySelector("#capture"), {scale: 2}).then(canvas => {
        const link = document.createElement('a')
        link.href = canvas.toDataURL()
        link.download = 'screenshot.png'
        link.click()
      })
  }
    }
  }
</script>

<style>
#table-container{
  overflow-y: scroll;
  height: 500px;
}
table {
    border-collapse: collapse;
    width: 100%;
}

th, td {
    border: 1px solid black;
    padding: 8px;
    text-align: left;
}

th {
    background-color: #f2f2f2;
}

</style>