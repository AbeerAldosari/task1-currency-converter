<template>
  <!-- Currency Converter UI -->
  <div class="container mt-5">
    <img alt="Vue logo" src="./assets/exchange.png" >
    <h1 class="text-center">Converter Currency</h1>

      <!-- From Currency Selection -->
    <div class="row">
        <div class="form-group">
          <label for="first-currency">From Currency:</label>
          <select class="form-control" name="first-currency" id="first-currency" v-model="currency_one">
             <!-- List of currency options -->
        <option value="USD">USD</option>
        <option value="AED">AED</option>
        <option value="AFN">AFN</option>
        <option value="ALL">ALL</option>
        <option value="AMD">AMD</option>
        <option value="ANG">ANG</option>
        <option value="AOA">AOA</option>
        <option value="ARS">ARS</option>
        <option value="AUD">AUD</option>
        <option value="AWG">ARS</option>
        <option value="AZN">AUD</option>
        <option value="BAM">BAM</option>
        <option value="BBD">BBD</option>
        <option value="BDT">BDT</option>
        <option value="BGN">BGN</option>
        <option value="BHD">BHD</option>
        <option value="BIF">BIF</option>
        <option value="BMD">BMD</option>
        <option value="BND">BND</option>
        <option value="BOB">BOB</option>
        <option value="BRL">BRL</option>
        <option value="BSD">BSD</option>
        <option value="BTN">BTN</option>
        <option value="BWP">BWP</option>
        <option value="BYN">BYN</option>
        <option value="BZD">BZD</option>
        <option value="CAD">CAD</option>
        <option value="CDF">CDF</option>
        <option value="CHF">CHF</option>
        <option value="CLP">CLP</option>
        <option value="CNY">CNY</option>
        <option value="COP">ARS</option>
        <option value="CRC">CRC</option>
        <option value="CUP">CUP</option>
        <option value="CVE">CVE</option>
        <option value="CZK">CZK</option>
        <option value="DJF">DJF</option>
        <option value="DKK">DKK</option>
        <option value="DOP">DOP</option>
        <option value="DZD">DZD</option>
        <option value="EGB">EGB</option>
        <option value="ERN">ERN</option>
        <option value="EUR">EUR</option>
        <option value="FJD">FGD</option>
        <option value="FKP">FKP</option>
        <option value="FOK">FOK</option>
        <option value="GBP">CLP</option>
        <option value="GEL">GEL</option>
        <option value="GGB">GGB</option>
        <option value="GHS">GHS</option>
        <option value="GIP">GIP</option>
        <option value="GMD">GMD</option>
        <option value="GNF">GNF</option>
        <option value="GTQ">GTQ</option>
        <option value="GYD">GYD</option>
        <option value="HKD">HKD</option>
        <option value="HNL">HNL</option>
        <option value="HRK">HRK</option>
        <option value="HTG">HTG</option>
        <option value="HUF">HUF</option>
        <option value="IDR">IDR</option>
        <option value="ILS">ILS</option>
        <option value="IMP">IMP</option>
        <option value="INR">INR</option>
        <option value="IQD">IQD</option>
        <option value="IRR">IRR</option>
        <option value="ISK">ISK</option>
        <option value="JEP">JEP</option>
        <option value="JMD">JMD</option>
        <option value="JOD">JOD</option>
        <option value="JPY">JPY</option>
        <option value="KES">KES</option>
        <option value="KGS">KGS</option>
        <option value="KHR">KHR</option>
        <option value="KID">KID</option>
        <option value="KMF">KMF</option>
        <option value="KRW">KRW</option>
        <option value="KWD">KWD</option>
        <option value="KYD">KYD</option>
        <option value="KZI">KZI</option>
        <option value="LAK">LAK</option>
        <option value="LBP">LBP</option>
        <option value="LKR">LKR</option>
        <option value="LRD">LRD</option>
        <option value="LSL">LSL</option>
        <option value="LYD">LYD</option>
        <option value="MAD">MAD</option>
        <option value="MDL">MDL</option>
        <option value="MGA">MGA</option>
        <option value="MKD">MKD</option>
        <option value="MMK">MMK</option>
        <option value="MNT">MNT</option>
        <option value="MOP">MOP</option>
        <option value="MRU">MRU</option>
        <option value="MUR">MUR</option>
        <option value="MVR">MVR</option>
        <option value="MWK">MWK</option>
        <option value="MXN">MXN</option>
        <option value="MYR">MYR</option>
        <option value="MZN">MZN</option>
        <option value="NAD">NAD</option>
        <option value="NGN">NGN</option>
        <option value="NIO">NIO</option>
        <option value="NOK">NOK</option>
        <option value="NPR">NPR</option>
        <option value="NZD">NZD</option>
        <option value="OMR">OMR</option>
        <option value="PAB">PAB</option>
        <option value="PGK">PGK</option>
        <option value="PEN">PEN</option>
        <option value="PHP">PHP</option>
        <option value="PKR">PKR</option>
        <option value="PLN">PLN</option>
        <option value="PYG">PYG</option>
        <option value="QAR">QAR</option>
        <option value="RON">RON</option>
        <option value="RUB">RUB</option>
        <option value="RWF">RWF</option>
        <option value="SAR">SAR</option>
        <option value="SBD">SBD</option>
        <option value="SCR">SCR</option>
        <option value="SDG">SDG</option>
        <option value="SEK">SEK</option>
        <option value="SGD">SGD</option>
        <option value="SHP">SHP</option>
        <option value="SLL">SLL</option>
        <option value="SOS">SOS</option>
        <option value="SRD">SRD</option>
        <option value="SSP">SSP</option>
        <option value="STN">STN</option>
        <option value="SYP">SYP</option>
        <option value="SZL">SZL</option>
        <option value="THB">THB</option>
        <option value="TJS">TJS</option>
        <option value="TMT">TMT</option>
        <option value="TND">TND</option>
        <option value="TOP">TOP</option>
        <option value="TRY">TRY</option>
        <option value="TTD">TTD</option>
        <option value="TVD">TVD</option>
        <option value="TWD">TWD</option>
        <option value="TZS">TZS</option>
        <option value="UAH">UAH</option>
        <option value="UGX">UGX</option>
        <option value="UYU">UYU</option>
        <option value="UZS">UZS</option>
        <option value="VES">VES</option>
        <option value="VND">VND</option>
        <option value="VUV">VUV</option>
        <option value="WST">WST</option>
        <option value="XAF">XAF</option>
        <option value="XCD">XCD</option>
        <option value="XDR">XDR</option>
        <option value="XOF">XOF</option>
        <option value="XPF">XPF</option>
        <option value="YER">YER</option>
        <option value="ZAR">ZAR</option>
        <option value="ZMW">ZMW</option>
        <option value="ZWL">ZWL</option>
      </select>
        </div> 
       </div>
        <!-- To Currency Selection -->
        <div class="form-group">
      <label for="second-currency">To Currency:</label>
      <select class="form-control" name="second-currency" id="second-currency" v-model="currency_two">
         <!-- List of currency options -->
        <option value="USD">USD</option>
        <option value="AED">AED</option>
        <option value="AFN">AFN</option>
        <option value="ALL">ALL</option>
        <option value="AMD">AMD</option>
        <option value="ANG">ANG</option>
        <option value="AOA">AOA</option>
        <option value="ARS">ARS</option>
        <option value="AUD">AUD</option>
        <option value="AWG">ARS</option>
        <option value="AZN">AUD</option>
        <option value="BAM">BAM</option>
        <option value="BBD">BBD</option>
        <option value="BDT">BDT</option>
        <option value="BGN">BGN</option>
        <option value="BHD">BHD</option>
        <option value="BIF">BIF</option>
        <option value="BMD">BMD</option>
        <option value="BND">BND</option>
        <option value="BOB">BOB</option>
        <option value="BRL">BRL</option>
        <option value="BSD">BSD</option>
        <option value="BTN">BTN</option>
        <option value="BWP">BWP</option>
        <option value="BYN">BYN</option>
        <option value="BZD">BZD</option>
        <option value="CAD">CAD</option>
        <option value="CDF">CDF</option>
        <option value="CHF">CHF</option>
        <option value="CLP">CLP</option>
        <option value="CNY">CNY</option>
        <option value="COP">ARS</option>
        <option value="CRC">CRC</option>
        <option value="CUP">CUP</option>
        <option value="CVE">CVE</option>
        <option value="CZK">CZK</option>
        <option value="DJF">DJF</option>
        <option value="DKK">DKK</option>
        <option value="DOP">DOP</option>
        <option value="DZD">DZD</option>
        <option value="EGB">EGB</option>
        <option value="ERN">ERN</option>
        <option value="EUR">EUR</option>
        <option value="FJD">FGD</option>
        <option value="FKP">FKP</option>
        <option value="FOK">FOK</option>
        <option value="GBP">CLP</option>
        <option value="GEL">GEL</option>
        <option value="GGB">GGB</option>
        <option value="GHS">GHS</option>
        <option value="GIP">GIP</option>
        <option value="GMD">GMD</option>
        <option value="GNF">GNF</option>
        <option value="GTQ">GTQ</option>
        <option value="GYD">GYD</option>
        <option value="HKD">HKD</option>
        <option value="HNL">HNL</option>
        <option value="HRK">HRK</option>
        <option value="HTG">HTG</option>
        <option value="HUF">HUF</option>
        <option value="IDR">IDR</option>
        <option value="ILS">ILS</option>
        <option value="IMP">IMP</option>
        <option value="INR">INR</option>
        <option value="IQD">IQD</option>
        <option value="IRR">IRR</option>
        <option value="ISK">ISK</option>
        <option value="JEP">JEP</option>
        <option value="JMD">JMD</option>
        <option value="JOD">JOD</option>
        <option value="JPY">JPY</option>
        <option value="KES">KES</option>
        <option value="KGS">KGS</option>
        <option value="KHR">KHR</option>
        <option value="KID">KID</option>
        <option value="KMF">KMF</option>
        <option value="KRW">KRW</option>
        <option value="KWD">KWD</option>
        <option value="KYD">KYD</option>
        <option value="KZI">KZI</option>
        <option value="LAK">LAK</option>
        <option value="LBP">LBP</option>
        <option value="LKR">LKR</option>
        <option value="LRD">LRD</option>
        <option value="LSL">LSL</option>
        <option value="LYD">LYD</option>
        <option value="MAD">MAD</option>
        <option value="MDL">MDL</option>
        <option value="MGA">MGA</option>
        <option value="MKD">MKD</option>
        <option value="MMK">MMK</option>
        <option value="MNT">MNT</option>
        <option value="MOP">MOP</option>
        <option value="MRU">MRU</option>
        <option value="MUR">MUR</option>
        <option value="MVR">MVR</option>
        <option value="MWK">MWK</option>
        <option value="MXN">MXN</option>
        <option value="MYR">MYR</option>
        <option value="MZN">MZN</option>
        <option value="NAD">NAD</option>
        <option value="NGN">NGN</option>
        <option value="NIO">NIO</option>
        <option value="NOK">NOK</option>
        <option value="NPR">NPR</option>
        <option value="NZD">NZD</option>
        <option value="OMR">OMR</option>
        <option value="PAB">PAB</option>
        <option value="PGK">PGK</option>
        <option value="PEN">PEN</option>
        <option value="PHP">PHP</option>
        <option value="PKR">PKR</option>
        <option value="PLN">PLN</option>
        <option value="PYG">PYG</option>
        <option value="QAR">QAR</option>
        <option value="RON">RON</option>
        <option value="RUB">RUB</option>
        <option value="RWF">RWF</option>
        <option value="SAR">SAR</option>
        <option value="SBD">SBD</option>
        <option value="SCR">SCR</option>
        <option value="SDG">SDG</option>
        <option value="SEK">SEK</option>
        <option value="SGD">SGD</option>
        <option value="SHP">SHP</option>
        <option value="SLL">SLL</option>
        <option value="SOS">SOS</option>
        <option value="SRD">SRD</option>
        <option value="SSP">SSP</option>
        <option value="STN">STN</option>
        <option value="SYP">SYP</option>
        <option value="SZL">SZL</option>
        <option value="THB">THB</option>
        <option value="TJS">TJS</option>
        <option value="TMT">TMT</option>
        <option value="TND">TND</option>
        <option value="TOP">TOP</option>
        <option value="TRY">TRY</option>
        <option value="TTD">TTD</option>
        <option value="TVD">TVD</option>
        <option value="TWD">TWD</option>
        <option value="TZS">TZS</option>
        <option value="UAH">UAH</option>
        <option value="UGX">UGX</option>
        <option value="UYU">UYU</option>
        <option value="UZS">UZS</option>
        <option value="VES">VES</option>
        <option value="VND">VND</option>
        <option value="VUV">VUV</option>
        <option value="WST">WST</option>
        <option value="XAF">XAF</option>
        <option value="XCD">XCD</option>
        <option value="XDR">XDR</option>
        <option value="XOF">XOF</option>
        <option value="XPF">XPF</option>
        <option value="YER">YER</option>
        <option value="ZAR">ZAR</option>
        <option value="ZMW">ZMW</option>
        <option value="ZWL">ZWL</option>
      </select>
    </div>
     
    <!-- Exchange Rate Information -->
    <div class="row">
      <div>
        <h4>1 {{currency_one}} = {{ rate }} {{ currency_two }}</h4>
      </div>
    </div>

      <!-- Amount to Convert -->
    <div class="form-group">
          <label for="input-one">Amount:</label>
          <input class="form-control" type="number" name="input-one" id="input-one" v-model="amountOne" @change="convertCurrency">
        </div>

   <!-- Converted Amount Display -->
    <div class="form-group">
      <label>Converted Amount:</label>
      <h2>{{ amountOne }} {{ currency_one }} = {{ amountTwo }} {{ currency_two }}</h2>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      // Data for currency converter
      currencies: {
        // List of currency codes and their respective conversion rates
       "USD":1,
  "AED":3.6725,
  "AFN":85.9494,
  "ALL":90.1886,
  "AMD":386.3240,
  "ANG":1.7900,
  "AOA":833.3862,
  "ARS":266.6713,
  "AUD":1.4678,
  "AWG":1.7900,
  "AZN":1.7005,
  "BAM":1.7413,
  "BBD":2.0000,
  "BDT":108.7494,
  "BGN":1.7409,
  "BHD":0.3760,
  "BIF":2820.2293,
  "BMD":1.0000,
  "BND":1.3220,
  "BOB":6.9094,
  "BRL":4.8075,
  "BSD":1.0000,
  "BTN":82.0718,
  "BWP":13.1624,
  "BYN":2.7650,
  "BZD":2.0000,
  "CAD":1.3180,
  "CDF":2335.2096,
  "CHF":0.8577,
  "CLP":818.2217,
  "CNY":7.1830,
  "COP":4020.4295,
  "CRC":538.0542,
  "CUP":24.0000,
  "CVE":98.1694,
  "CZK":21.1973,
  "DJF":177.7210,
  "DKK":6.6420,
  "DOP":55.9682,
  "DZD":134.3855,
  "EGP":30.8980,
  "ERN":15.0000,
  "ETB":55.0051,
  "EUR":0.8903,
  "FJD":2.1900,
  "FKP":0.7660,
  "FOK":6.6420,
  "GBP":0.7659,
  "GEL":2.5664,
  "GGP":0.7660,
  "GHS":11.5229,
  "GIP":0.7660,
  "GMD":62.8693,
  "GNF":8501.5029,
  "GTQ":7.8357,
  "GYD":210.1530,
  "HKD":7.8130,
  "HNL":24.5904,
  "HRK":6.7080,
  "HTG":138.0267,
  "HUF":332.5320,
  "IDR":14991.7418,
  "ILS":3.6065,
  "IMP":0.7660,
  "INR":82.0719,
  "IQD":1307.7396,
  "IRR":41992.6251,
  "ISK":130.2495,
  "JEP":0.7660,
  "JMD":154.4891,
  "JOD":0.7090,
  "JPY":138.7945,
  "KES":141.7300,
  "KGS":87.8568,
  "KHR":4135.0625,
  "KID":1.4677,
  "KMF":438.0008,
  "KRW":1262.6921,
  "KWD":0.3063,
  "KYD":0.8333,
  "KZT":443.8032,
  "LAK":19093.6567,
  "LBP":15000.0000,
  "LKR":322.0642,
  "LRD":183.9153,
  "LSL":17.8733,
  "LYD":4.7397,
  "MAD":9.7338,
  "MDL":18.0190,
  "MGA":4472.2492,
  "MKD":54.7756,
  "MMK":2096.3987,
  "MNT":3438.3990,
  "MOP":8.0477,
  "MRU":35.9542,
  "MUR":45.1613,
  "MVR":15.4391,
  "MWK":1052.3767,
  "MXN":16.7476,
  "MYR":4.5408,
  "MZN":64.3144,
  "NAD":17.8733,
  "NGN":764.8258,
  "NIO":36.5514,
  "NOK":10.0553,
  "NPR":131.3149,
  "NZD":1.5902,
  "OMR":0.3845,
  "PAB":1.0000,
  "PEN":3.5607,
  "PGK":3.5706,
  "PHP":54.4328,
  "PKR":278.9363,
  "PLN":3.9554,
  "PYG":7267.1600,
  "QAR":3.6400,
  "RON":4.3903,
  "RSD":104.2811,
  "RUB":90.6996,
  "RWF":1220.7387,
  "SAR":3.7500,
  "SBD":8.4998,
  "SCR":13.2974,
  "SDG":538.4462,
  "SEK":10.2145,
  "SGD":1.3220,
  "SHP":0.7660,
  "SLE":19.7124,
  "SLL":19712.4017,
  "SOS":569.8327,
  "SRD":38.2343,
  "SSP":995.3312,
  "STN":21.8124,
  "SYP":2509.4679,
  "SZL":17.8733,
  "THB":34.0962,
  "TJS":10.9147,
  "TMT":3.5000,
  "TND":3.0303,
  "TOP":2.2934,
  "TRY":26.9376,
  "TTD":6.7551,
  "TVD":1.4677,
  "TWD":30.9767,
  "TZS":2443.0899,
  "UAH":36.7973,
  "UGX":3676.8642,
  "UYU":38.0623,
  "UZS":11732.3797,
  "VES":28.8123,
  "VND":23642.8828,
  "VUV":117.4731,
  "WST":2.7007,
  "XAF":584.0011,
  "XCD":2.7000,
  "XDR":0.7381,
  "XOF":584.0011,
  "XPF":106.2417,
  "YER":250.1973,
  "ZAR":17.8729,
  "ZMW":19.0106,
  "ZWL":4878.8310
},
      currency_one: "USD",
      currency_two: "EUR",
      rate: "",
      amountOne: 1,
      amountTwo: 1,
    };
  },
  methods: {
    // Method to convert currency based on user input
    convertCurrency() {
      this.rate = this.currencies[this.currency_two];
      this.amountTwo = (this.amountOne * this.rate).toFixed(2);
    },
  },
  watch: {
    // Watch for changes in currency selection or amount input
    currency_one: "convertCurrency",
    currency_two: "convertCurrency",
    amountOne: "convertCurrency",
  },
  created() {
    // Convert initial amount on component creation
    this.convertCurrency();
  },
};
</script>

<style>
/* CSS Styles for Currency Converter UI */
/* ... CSS styles for the UI components ... */
html {
  background: #f4f4f4;
}

#app {
  display: flex;
  flex-direction: column;
  align-items: center;
  align-content: center;
  width: 100%;
  height: 100%;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

h1 {
  color: #454f69;
}

img {
  width: 150px;
}

.container {
  width: 35%;
  height: 110%;
  padding: 30px;
  display: flex;
  flex-direction: column;
  align-items: center;
  align-content: center;
  text-align: center;
  margin: 50px;
  border: 3px rgb(21, 99, 58) solid;
  border-radius: 50px;
  box-shadow: 10px 5px 5px rgba(0, 0, 0, 0.5); /* Added shadow effect */
}

.container-two {
  display: flex;
  align-items: center;
  justify-content: space-between;
  width: 50%;
  padding: 2px;
}

select {
  padding: 5px;
  margin: 5px;
  border: 1px solid rgba(0, 0, 0, 0.5);
}

input {
  padding: 5px;
  margin: 5px;
  border: 1px solid rgba(0, 0, 0, 0.5);
  outline: none;
  font-size: 18px;
}

#basevalue {
  font-weight: 500;
}
</style>