<template>
  <footer class="bg-[#012430] text-white pt-16 pb-8">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Main Footer Content -->
      <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8 mb-12 text-center md:text-left">
        <!-- Company Info & Logo -->
        <div>
          <div class="mb-6">
            <NuxtLink to="/" class="inline-block">
              <img src="/assets/img/elevation-logo2.png" alt="Elevation Consulting Logo"
                class="h-12 md:h-14 lg:h-16 drop-shadow-lg" />
            </NuxtLink>
          </div>
          <p class="text-gray-300 mb-6 max-w-md mx-auto md:mx-0">
            We are a boutique consulting firm dedicated to strengthening Nigeria's and Africa's private sector through
            enterprise support, capacity development, and strategic advisory.
          </p>
          <div class="flex space-x-4 justify-center md:justify-start">
            <a href="https://web.facebook.com/people/Elevation-Consulting/100066769537474/?rdid=U7skCPT9dg2Lv9yE&share_url=https%3A%2F%2Fweb.facebook.com%2Fshare%2F19AcbTS8GT%2F%3F_rdc%3D1%26_rdr"
              target="_blank" rel="noopener noreferrer"
              class="text-gray-400 hover:text-[#0077AA] transition-colors duration-200">
              <Icon name="lucide:facebook" class="w-6 h-6" />
            </a>
            <a href="https://www.linkedin.com/in/elevation-consulting" target="_blank" rel="noopener noreferrer"
              class="text-gray-400 hover:text-[#0077AA] transition-colors duration-200">
              <Icon name="lucide:linkedin" class="w-6 h-6" />
            </a>
            <a href="https://www.instagram.com/consultingelevation" target="_blank" rel="noopener noreferrer"
              class="text-gray-400 hover:text-[#0077AA] transition-colors duration-200">
              <Icon name="lucide:instagram" class="w-6 h-6" />
            </a>
            <a href="https://wa.me/2349026944592" target="_blank" rel="noopener noreferrer"
              class="hover:opacity-80 transition-opacity duration-200">
              <img src="/assets/img/whatsapp.png" alt="WhatsApp" class="w-6 h-6" />
            </a>
          </div>
        </div>

        <!-- Quick Links (Navbar Items) -->
        <div>
          <h3 class="text-lg font-semibold mb-6 text-white border-b border-[#0077AA] pb-2">Quick Links</h3>
          <ul class="grid grid-cols-1 lg:grid-cols-2 gap-x-8 gap-y-3">
            <li>
              <NuxtLink to="/about-us" class="text-gray-300 hover:text-[#0077AA] transition-colors duration-200">
                About Us
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/consulting" class="text-gray-300 hover:text-[#0077AA] transition-colors duration-200">
                Consulting
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/advisory" class="text-gray-300 hover:text-[#0077AA] transition-colors duration-200">
                Advisory
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/training" class="text-gray-300 hover:text-[#0077AA] transition-colors duration-200">
                Training
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/business-development"
                class="text-gray-300 hover:text-[#0077AA] transition-colors duration-200">
                Business Development
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/monitoring-evaluation"
                class="text-gray-300 hover:text-[#0077AA] transition-colors duration-200">
                Monitoring & Evaluation
              </NuxtLink>
            </li>
            <li>
              <NuxtLink to="/programs-events" class="text-gray-300 hover:text-[#0077AA] transition-colors duration-200">
                Programs & Events
              </NuxtLink>
            </li>
          </ul>
        </div>

        <!-- Contact Information -->
        <div>
          <h3 class="text-lg font-semibold mb-6 text-white border-b border-[#0077AA] pb-2">Contact Us</h3>
          <ul class="space-y-4">
            <li class="flex items-start justify-center md:justify-start">
              <Icon name="lucide:map-pin" class="w-5 h-5 mt-0.5 mr-3 text-[#0077AA] flex-shrink-0" />
              <span class="text-gray-300 text-left">20 Lewis Street Lagos Island,
                Lagos, Nigeria</span>
            </li>
            <li class="flex items-center justify-center md:justify-start">
              <Icon name="lucide:phone" class="w-5 h-5 mr-3 text-[#0077AA] flex-shrink-0" />
              <span class="text-gray-300">(+234) 803 337 7366, <br>(+234) 803 878 6056</br><br>(+234)
                902 694 4592</br></span>
            </li>
            <li class="flex items-center justify-center md:justify-start">
              <Icon name="lucide:mail" class="w-5 h-5 mr-3 text-[#0077AA] flex-shrink-0" />
              <span class="text-gray-300">info@elevationconsulting.com.ng,<br>
                elevationconsultingsg@gmail.com</br></span>
            </li>
            <li class="flex items-center justify-center md:justify-start">
              <Icon name="lucide:clock" class="w-5 h-5 mr-3 text-[#0077AA] flex-shrink-0" />
              <span class="text-gray-300">Mon - Fri: 8:00 AM - 6:00 PM</span>
            </li>
          </ul>
        </div>
      </div>

      <!-- Bottom Footer with Darker Background -->
      <div class="bg-gray-950 -mx-4 sm:-mx-6 lg:-mx-8 px-4 -my-6 sm:px-6 lg:px-8 border-t border-gray-700 pt-6 pb-6">
        <div
          class="flex flex-col md:flex-row justify-between items-center space-y-4 md:space-y-0 text-center md:text-left">
          <p class="text-gray-400 text-sm">
            © {{ new Date().getFullYear() }} Elevation Consulting. All rights reserved.
          </p>
          <div class="flex flex-col sm:flex-row items-center space-y-2 sm:space-y-0 sm:space-x-6">
            <button @click="showPrivacyPolicy = true"
              class="text-gray-400 hover:text-white transition-colors duration-200 text-sm">
              Privacy Policy
            </button>
            <button @click="showTermsOfService = true"
              class="text-gray-400 hover:text-white transition-colors duration-200 text-sm">
              Terms of Service
            </button>
            <div class="text-gray-400 text-sm">
              Design & Development by
              <a href="https://tekfolio.ng" target="_blank" rel="noopener noreferrer"
                class="text-[#0077AA] hover:text-white transition-colors duration-200">
                Tekfolio
              </a>
            </div>
          </div>
        </div>
      </div>

      <!-- Modal Components -->
      <PrivacyPolicyModal v-model="showPrivacyPolicy" />
      <TermsOfServiceModal v-model="showTermsOfService" />
    </div>

    <!-- WhatsApp Floating Button -->
    <a href="https://wa.me/2349026944592" target="_blank" rel="noopener noreferrer"
      class="fixed bottom-6 right-6 z-50 bg-[#29a71a] p-4 rounded-full shadow-2xl hover:scale-110 transition-all duration-300 group">
      <img src="/assets/img/whatsapp.png" alt="WhatsApp" class="w-12 h-12" />
      <span
        class="absolute right-full mr-3 top-1/2 -translate-y-1/2 bg-gray-900 text-white px-3 py-2 rounded-lg text-sm whitespace-nowrap opacity-0 group-hover:opacity-100 transition-opacity duration-300 pointer-events-none">
        Chat with us on WhatsApp
      </span>
    </a>
  </footer>
</template>

<script setup>
import { ref } from 'vue';
import PrivacyPolicyModal from '~/components/home/PrivacyPolicyModal.vue';
import TermsOfServiceModal from '~/components/home/TermsOfServiceModal.vue';

const showPrivacyPolicy = ref(false);
const showTermsOfService = ref(false);
</script>
