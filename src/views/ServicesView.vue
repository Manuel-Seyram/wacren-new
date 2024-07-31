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

//Awareness

function showAwareness() {
  Modal.fire({
    title: "Awareness",
    text: " WACREN CSIRT participates in any awareness campaign from TrustBroker Africa(TBA) and directly to its constituency at other times.",
  });
}
//Alerts
function showAlerts() {
  Modal.fire({
    title: "Alerts and Warnings",
    text: "This service consists of the publication of information describing an attack, an alert, a threat, etc. and the provision of short-term action recommendations that allow it to face the problem.",
  });
}
//Incidents
function showIncidents() {
  Modal.fire({
    title: "Incident Handling",
    text: "The service entails managing and mitigating security incidents.",
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
          Our Services
        </p>
      </div>
      <div class="w-full px-5 xl:px-0">
        <div class="container mx-auto max-w-5xl">
          <div
            class="md:flex justify-between mt-10 text-center space-x-1 xl:space-x-0 space-y-2 xl:space-y-0"
          >
            <button
              @click="showAwareness"
              class="bg-blue-500 w-40 h-12 rounded-lg font-nunito shadow-lg hover:shadow-lg hover:shadow-blue-600 hover:bg-blue-600"
            >
              Awareness
            </button>
            <button
              @click="showAlerts"
              class="bg-blue-500 w-40 h-12 rounded-lg font-nunito shadow-lg hover:shadow-lg hover:shadow-blue-600 hover:bg-blue-600"
            >
              Alerts and Warnings
            </button>
            <button
              @click="showIncidents"
              class="bg-blue-500 w-40 h-12 rounded-lg font-nunito shadow-lg hover:shadow-lg hover:shadow-blue-600 hover:bg-blue-600"
            >
              Incident Handling
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
