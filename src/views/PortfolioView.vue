<script>
export default {
  data() {
    return {
      activeTab: 1,
      items: [
        {
          id: 1,
          name: 'Spirit Jack Daniel',
          imageUrl: 'xabi1',
          status: 'Desain sureal dan petualangan menampilkan botol besar Jack Daniels berwarna biru sebagai pusat perhatian di lanskap pegunungan yang megah, lengkap dengan air terjun dan bulan biru raksasa. Seekor hiu putih besar muncul dengan dramatis di belakang botol, menciptakan suasana fantasi epik tentang kekuatan dan eksplorasi yang tak terduga.',
          tech: 'Photoshop',
          github: 'https://www.instagram.com/p/DOxV0V1D268/?utm_source=ig_web_copy_link&igsh=MzRlODBiNWFlZA==',
          demo: 'https://files.catbox.moe/n0u85f.jpg'
        },
        {
          id: 2,
          name: 'Unleash The Beast',
          imageUrl: 'xabi2',
          status: 'Poster ini menampilkan kaleng minuman Monster Energy dengan fokus sentral, logo cakar neon hijau yang bercahaya terang di tengah latar belakang fantasi yang gelap dan suram. Di belakang kaleng, sebuah makhluk fantasi raksasa berwarna gelap, mungkin naga atau monster purba, berdiri di atas puing-puing berbatu. Makhluk itu melengkung dan tampak seperti penjaga atau representasi dari energi yang dilepaskan. Suasana keseluruhannya adalah misterius dan kekuatan mentah, menghubungkan merek minuman dengan tema monster dan kekuatan yang "primitif" atau kuno. Desainnya sangat dramatis dengan kontras antara warna hijau neon yang cerah dan palet gelap (hitam, abu-abu, hijau lumut) dari lingkungan sekitarnya.',
          tech: 'photoshop',
          github: 'https://www.instagram.com/p/DOz7bYYj2oR/?utm_source=ig_web_copy_link&igsh=MzRlODBiNWFlZA==',
          demo: 'https://files.catbox.moe/ynyx0s.jpg'
        },
        {
          id: 3,
          name: 'Tropicana Apple Juice',
          imageUrl: 'xabi3',
          status: 'Iklan yang hidup dan segar untuk jus apel Tropicana. Kemasan jus diposisikan di tengah, dikelilingi oleh apel merah yang berlimpah dan dedaunan subur. Latar belakang pemandangan alam hijau cerah dengan sungai kecil dan kupu-kupu, menggarisbawahi tema alami, keaslian, dan kesegaran produk yang mengalir.',
          tech: 'Photoshop',
          github: 'https://www.instagram.com/p/DOxfz_Rj2sC/?utm_source=ig_web_copy_link&igsh=MzRlODBiNWFlZA==',
          demo: 'https://files.catbox.moe/p7jhgj.jpg'
        },
        {
          id: 4,
          name: 'Chanel Coco Noir',
          imageUrl: 'xabi4',
          status: 'Desain iklan yang sangat minimalis dan mewah, berfokus pada botol parfum Chanel Coco Noir yang hitam pekat. Diletakkan di tengah komposisi yang didominasi oleh nuansa hitam gelap dengan latar belakang geometris abstrak, menciptakan kesan elegan, kedalaman, dan misteri abadi.',
          tech: 'Photoshop',
          github: 'https://www.instagram.com/p/DOusWLyj_9X/?utm_source=ig_web_copy_link&igsh=MzRlODBiNWFlZA==',
          demo: 'https://files.catbox.moe/oub1hk.jpg'
        },
        {
          id: 5,
          name: 'Summoners Ascent',
          imageUrl: 'xabi6',
          status: 'Seni fantasi gelap yang dramatis menampilkan sosok pemanggil berjubah berdiri di puncak tebing berbatu, mengangkat tangan ke langit. Mereka memanggil dua makhluk bersayap raksasa(mirip pterodactyl/ naga) yang muncul di depan bulan purnama biru cemerlang yang sangat besar. Pencahayaan didominasi oleh kontras tajam antara biru dingin dan kegelapan, menciptakan suasana epik dan misterius.',
          tech: 'Photoshop',
          github: 'https://www.instagram.com/p/DPAwrv7D8qV/?utm_source=ig_web_copy_link&igsh=MzRlODBiNWFlZA==',
          demo: 'https://files.catbox.moe/9vy6rk.jpg'
        }
      ]
    };
  }
}
</script>
<template>
  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article data-page="about">
      <header>
        <div
          class="text-2xl font-bold text-white mb-10 fadein-bot title-section flex items-center justify-center flex-col">
          <!-- <div class="h-[1px] w-10 bg-amber-200 md:w-20 aos-init aos-animate"></div> -->
          <h4>Past Project Experience</h4>
          <h4 class="text-base font-normal text-transparent bg-clip-text bg-gradient-to-r from-slate-100 to-amber-300">
            Explore the projects I've worked on so far</h4>
        </div>
      </header>
      <section>
        <div>
          <div
            class="grid grid-cols-1 gap-4 pb-32 md:grid-cols-3 md:gap-3 xl:grid-cols-3 xl:gap-3 2xl:gap-5 fade-zoom-in">
            <div v-for="item in items" :key="item.id">
              <div
                class="item-card flex flex-col items-center gap-2 rounded bg-[#1e1e1f] hover:bg-[#282828] border border-[#383838] rounded-xl text-amber-50 md:gap-3 px-5 py-5 lg:px-5 ">
                <div class="flex h-12 w-12 items-center justify-center p-0 h-full w-full lg:p-0 zoom-in">
                  <img alt="HTML" loading="lazy" decoding="async" data-nimg="1"
                    class="drop-shadow-xl rounded rounded-xl" :src="'/img/portfolio-' + item.imageUrl + '.jpg'">
                </div>
                <div class="w-full flex flex-col gap-2 items-center text-sm md:text-base lg:text-lg">
                  <div class="title-text font-medium text-secondary">{{ item.name }}
                  </div>
                  <div class="w-full text-left text-[10px] text-[#c1c1c1] md:text-xs lg:text-sm">
                    {{ item.status }}</div>
                  <div class="w-full mt-4 text-normal text-sm text-left text-amber-200">
                    {{ item.tech }}
                  </div>
                  <div class="w-full flex justify-end">
                    <div class="flex cursor-pointer items-end gap-2 text-primary">
                      <a v-if="item.github !== 'null'" :href="item.github" target="_blank" rel="noreferrer"
                        title="View github repository" class="transition-all hover:text-accent">
                        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none"
                          stroke="#ffffff" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"
                          class="lucide lucide-instagram-icon lucide-instagram">
                          <rect width="20" height="20" x="2" y="2" rx="5" ry="5" />
                          <path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z" />
                          <line x1="17.5" x2="17.51" y1="6.5" y2="6.5" />
                        </svg></a>
                      <a v-if="item.demo !== 'null'" :href="item.demo" target="_blank" rel="noreferrer"
                        title="View finished project" class="transition-all hover:text-accent">
                        <svg stroke="currentColor" fill="none" stroke-width="2" viewBox="0 0 24 24"
                          stroke-linecap="round" stroke-linejoin="round" height="18" width="18"
                          xmlns="http://www.w3.org/2000/svg">
                          <path d="M18 13v6a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V8a2 2 0 0 1 2-2h6"></path>
                          <polyline points="15 3 21 3 21 9"></polyline>
                          <line x1="10" y1="14" x2="21" y2="3"></line>
                        </svg></a>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </article>
  </div>
</template>

<style>
.item-card:hover {
  transition: transform 0.3s ease;
  transform: translateY(-8px);
}

svg:hover {
  stroke: #ffdb70;
}

@keyframes fadeZoomIn {
  0% {
    opacity: 0;
    transform: scale(0.5);
  }

  100% {
    opacity: 1;
    transform: scale(1);
  }
}

/* Menggunakan animasi pada elemen yang diinginkan */
.fade-zoom-in {
  animation: fadeZoomIn 1s ease-in-out;
}
</style>
