<script setup>
import Swal from "sweetalert2";
import "sweetalert2/dist/sweetalert2.min.css";

const Modal = Swal.mixin({
  allowOutsideClick: true,
  showConfirmButton: false,
  showCloseButton: true,
  width: 400,
  heightAuto: true,
});

//WHO WE ARE

function showWho() {
  Modal.fire({
    title: "WHO WE ARE",
    text: " WACREN CSIRT participates in any awareness campaign from TrustBroker Africa(TBA) and directly to its constituency at other times.",
  });
}
//MISSION
function showMission() {
  Modal.fire({
    title: "MISSION",
    text: "“Maintain business continuity in our constituency by promoting awareness, rapid intervention and efficient incident handling” WACREN CSIRT WACREN CSIRT's mission is to serve as the front-line defender of WACREN and assist member NRENs in building or maintaining their CSIRT and cybersecurity digital assets (see constituency) by swiftly detecting, analyzing, and mitigating cybersecurity threats. Swift response to security incidents with speed, precision and expertise is the team's commitment. The actions and efficiency of the team are to satisfy the objective of promoting CSIRT services as an added value to WACREN's portfolio of products. By fostering a culture of resilience, promoting awareness, and implementing best practices, we aim to fortify our systems, protect sensitive data, and sustain uninterrupted operations. Our commitment is to uphold the trust of stakeholders and navigate the dynamic cybersecurity landscape with unwavering dedication. Through collaborative efforts, continuous improvement, and knowledge sharing, our mission is to ensure our systems' integrity, confidentiality, and availability, fortifying trust and stability in our digital environment.",
  });
}
//AFFILIATION
function showAffiliation() {
  Modal.fire({
    title: "SPONSORING & AFFILIATION",
    text: "The CSIRT is sponsored and affiliated with WACREN. WACREN mandates that its activities be executed within the scope of the constituency.",
  });
}

//AUTHORITY
function showAuthority() {
  Modal.fire({
    title: "AUTHORITY",
    text: "WACREN) supports interconnections and fosters collaboration between R&E institutions in the region and international peers by building and operating a world-class network infrastructure, developing state-of-the-art services, promoting collaboration among national, regional, and international R&E communities, and building the human capacity of the REN community. WACREN was constituted in 2010, and membership is open to all 22 countries in the region. It currently has 13 participating National Research and Education Networks (NRENs) from Benin, Burkina Faso, Cameroon, Chad, Cote d’Ivoire, Gabon, Ghana, Guinea, Mali, Niger, Nigeria, Senegal, and Togo. WACREN deploys cloud-based infrastructure to ease technological challenges experienced by many of its members. The CSIRT has the authority to oversee and make recommendations regarding the incident mitigation domain. The CSIRT will execute its duties within the scope of this Charter, as informed by any applicable laws, regulations, directives, and any additional assignments of responsibility from external governance bodies.",
  });
}
</script>

<template>
  <div class="min-h-screen flex flex-col bg-blue-400">
    <!-- Main content -->
    <div class="flex-grow">
      <div class="w-full h-48 bg-white">
        <p
          class="font-nunito font-bold tracking-wider text-center text-3xl uppercase pt-7"
        >
          About Us
        </p>
      </div>
      <div class="w-full px-5 xl:px-0">
        <div class="container mx-auto max-w-5xl">
          <div
            class="md:flex justify-between mt-10 text-center space-x-1 xl:space-x-0 space-y-2 xl:space-y-0"
          >
            <button
              @click="showWho"
              class="bg-blue-500 w-40 h-12 rounded-lg font-nunito uppercase hover:shadow-lg hover:shadow-blue-600 hover:bg-blue-600"
            >
              Who we are
            </button>
            <button
              @click="showMission"
              class="bg-blue-500 w-40 h-12 rounded-lg font-nunito uppercase hover:shadow-lg hover:shadow-blue-600 hover:bg-blue-600"
            >
              Mission
            </button>
            <button
              @click="showAffiliation"
              class="bg-blue-500 w-40 h-12 rounded-lg font-nunito uppercase hover:shadow-lg hover:shadow-blue-600 hover:bg-blue-600"
            >
              Sponsoring & Affiliation
            </button>
            <button
              @click="showAuthority"
              class="bg-blue-500 w-40 h-12 rounded-lg font-nunito uppercase hover:shadow-lg hover:shadow-blue-600 hover:bg-blue-600"
            >
              Authority
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
