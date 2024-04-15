<template>
  <div>
    <div>账号切换</div>
    <button @click="sici()" type="default" size="mini">sici</button>
    <button @click="wjl()" type="default" size="mini">王经理</button>
    <button @click="zzjl()" type="default" size="mini">张总经理</button>
    <button @click="admin()" type="default" size="mini">admin</button>
    <div>当前token：{{ token }}</div>
  </div>
</template>

<script>
export default {
  name: "Test",

  data() {
    return {
      token: ''
    };
  },

  created(){
    this.token = window.localStorage.getItem('token')
  },

  methods: {
    admin() {
      window.localStorage.setItem('token', '');
      let token = 'eyJhbGciOiJIUzUxMiIsInppcCI6IkdaSVAifQ.H4sIAAAAAAAAAKtWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDM3tzQxNDM01VEqLU4t8kwBikGYeYm5qUAtiSm5mXlKtQAjn-tfQgAAAA.dKczZ7BKISa_s3zV1VxVN2Yk7bSqRawbIUp1GVXDhpxD4n-jbrE-3UmruA_MM47H_OcLODk1R2TxI6HTPxnA-Q'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    },

    sici() {
      window.localStorage.setItem('token', '');
      let token = 'eyJ6aXAiOiJHWklQIiwiYWxnIjoiSFM1MTIifQ.H4sIAAAAAAAA_6tWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDc0NjYxNDc111EqLU4t8kxRsjIygLDzEnNTgXqKM5MzlWoBjg4MlkIAAAA.GZHrogQqxkaXCu6K8eVZg6Cy6aQBMU7hnkHDUg_fi6R27J0tYV3hcRJ9wBhx2gmNCtRrJtPWqg-BVmFEgRJ4NQ'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    },

    zzjl() {
      window.localStorage.setItem('token', '');
      let token = 'eyJ6aXAiOiJHWklQIiwiYWxnIjoiSFM1MTIifQ.H4sIAAAAAAAA_6tWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDc0NjYxNDcw1lEqLU4t8kxRsjIyh7DzEnNTgXqqMhLz0pVqAUBjJwBDAAAA.oKwRiAHWSNv-d2B_e7corq5yLo7Lbk7xVaRxSClHoWNunO-eo2TG5ZeuJIeTWrlz_SXRgie-8oFp03ZocJs57A'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    },

    wjl() {
      window.localStorage.setItem('token', '');
      let token = 'eyJ6aXAiOiJHWklQIiwiYWxnIjoiSFM1MTIifQ.H4sIAAAAAAAA_6tWKi5NUrJScgwN8dANDXYNUtJRSq0oULIyNDc0NjYxMDa30FEqLU4t8kxRsjKCsvMSc1OBesoT89KVagELcDEzQgAAAA.hja5YnslRwiH24hF05eCbPACjEqFcEm9PklL4qPS7AwyK04FvuGSA-cIiK2Flh131HJqAANyW1RTQTwIeLWGMw'
      window.localStorage.setItem('token', token);
      this.token = window.localStorage.getItem('token')
    }
  }
}
</script>
