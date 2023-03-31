<template>
  <vue-whatsapp-widget
    phoneNumber="+5521967543780"
    textReply="Geralmente responde em menos de 1h"
    messages="['Olá! Como posso te ajudar?', 'Olá, aguarde que em breve um dos nossos atenderá você!']"
    companyName="Agência Always"
  />
</template>
<script>
import VueWhatsappWidget from "vue-whatsapp-widget";
components: {
  VueWhatsappWidget;
}
</script>
