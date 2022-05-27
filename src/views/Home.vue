<template>
  <v-app
    id="home"
    :style="{ background: $vuetify.theme.themes.light.background }"
  >
    <nav-bar />
    <v-container fluid>
      <v-row class="homeprofile">
        <v-col cols="8">
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <!-- <h1 class="yellow--text" id="welcome">WELC</h1> -->

          <!-- <v-img src="../assets/header.jpeg" contain max-height="500"></v-img> -->
        </v-col>
        <v-col cols="4">
          <br>
          <br>
          <!-- <h1 class="yellow--text" id="welcome">ME!!!!</h1> -->
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br><br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
          <br>
        </v-col>
      </v-row>



      <!-- About Me Start -->
      <v-col cols="12" class="padd">
          <div class="first" id="about">
            <h2 class="black--text">About Me</h2>
            <v-col cols="12">
              <div class="child">
                <h3 align="center">Hello, I'm Susiana Sunjaya!<br></h3>
                <p align="center">I enjoy learning new things. 
                I always find motivation in the little things around me.<br> 
                That's what makes me a person who never gives up. <br> 
                I am good at team work and can give opinions to help the team make the best decisions.<br> 
                I am currently interested in data management and data analysis.<br> 
                I hope I can make a good impact in that field in the future.<br> 
                </p>
                <p>If you want to work with me or just want to have a disscussion, please contact me :D
                </p>
              </div>
            </v-col>
            <h2 class="black--text">Education</h2>
            <v-col cols="12">
              <div class="child">
                <v-card elevation="5" outlined shaped  width="350">
                  <v-card-title>Budya Wacana High School</v-card-title>
                  <v-card-subtitle>Science Class | 2016 - 2019</v-card-subtitle>
                  <v-card-text>Best Graduate of Science Class 2019</v-card-text>
                </v-card>
              </div>
              <div class="child">
                <v-card elevation="5" outlined shaped  width="350">
                  <v-card-title>Duta Wacana Christian Univeristy</v-card-title>
                  <v-card-subtitle>Computer Science | 2019 - Now</v-card-subtitle>
                  <v-card-text>GPA : 3.89</v-card-text>
                </v-card>
              </div>
            </v-col>
            <h2 class="black--text">Achievements</h2>
              <v-col cols="12">
                <div class="child">
                  <v-card elevation="5" outlined shaped  width="350" height="130">
                    <v-card-title>The Winner of OSC 2018</v-card-title>
                    <v-card-subtitle>medcom.id</v-card-subtitle>
                  </v-card>
                </div>
                <div class="child">
                  <v-card elevation="5" outlined shaped  width="350" height="130">
                    <v-card-title>2nd Runner Up of <br>EAD's Writting Competition</v-card-title>
                    <v-card-subtitle>FKIP Universitas Sanata Dharma</v-card-subtitle>
                  </v-card>
                </div>
              </v-col>
            <h2 class="black--text">Ability</h2>
            <div id="ability">
                <div class="child">
                <img src="../assets/python.jpg" alt="python" width="80px">
                <img src="../assets/html.jpg" alt="html" width="80px">
                <img src="../assets/css.jpg" alt="css" width="80px">
                <img src="../assets/php.png" alt="php" width="80px">
                <img src="../assets/js.jpg" alt="js" width="80px">
                <img src="../assets/java.png" alt="java" width="80px">
                <img src="../assets/MySQL.png" alt="mysql" width="80px">

                </div>                
            </div>

            <h2 class="black--text">Experience</h2>
            <v-col cols="12">
              <div class="child">
                <v-container fluid>
                  <v-row justify="center">
                    <v-expansion-panels popout>
                      <v-expansion-panel
                      v-for="(message, i) in messages"
                      :key="i"
                      hide-actions
                    >
                      <v-expansion-panel-header>
                        <v-row align="center" class="spacer" no-gutters>
                          <v-col cols="4" sm="2" md="1">
                            <v-avatar size="36px">
                              <img
                                v-if="message.avatar"
                                alt="Avatar"
                                src="../assets/profile.png"
                              >
                              <v-icon
                                v-else
                                :color="message.color"
                                v-text="message.icon"
                              ></v-icon>
                            </v-avatar>
                          </v-col>

                          <v-col class="hidden-xs-only" sm="5" md="3">
                            <strong v-html="message.name"></strong>
                            <span
                              v-if="message.total"
                              class="grey--text"
                            >
                              &nbsp;({{ message.total }})
                            </span>
                          </v-col>

                          <v-col class="text-no-wrap" cols="5" sm="3">
                            <v-chip
                              v-if="message.new"
                              :color="`${message.color} lighten-4`"
                              class="ml-0 mr-2 black--text"
                              label
                              small
                            >
                              {{ message.new }} new
                            </v-chip>
                            <strong v-html="message.title"></strong>
                          </v-col>

                        </v-row>
                      </v-expansion-panel-header>

                      <v-expansion-panel-content>
                        <v-divider></v-divider>
                        <!-- <v-card-text v-text="detailexp"></v-card-text> -->
                        <v-card-text>
                          <ul>
                            <li v-text="message.detail1"></li>
                            <li v-text="message.detail2"></li>
                          </ul>
                        </v-card-text>

                      </v-expansion-panel-content>
                    </v-expansion-panel>
                  </v-expansion-panels>
                </v-row>
              </v-container>
              </div>

            </v-col>
          <br><br><br>


            <h2 class="black--text">Organization</h2>
              <v-container>
                <v-row justify="space-around">
                  <v-timeline align-top dense>
                    <v-timeline-item
                      v-for="organization in organizations"
                      :key="organization.year"
                      :color="organization.color"
                      small
                    >
                    <div align="left">
                      <div class="font-weight-normal">
                        <strong>{{ organization.organization }}</strong> <br>
                        {{ organization.title }}
                      </div>
                      <div>{{ organization.year }}</div>
                    </div>
                    </v-timeline-item>
                  </v-timeline>

                </v-row>
              </v-container>

            <!-- <h2 class="blue--text">Event</h2>
              <v-col cols="12">
              <div class="child">
                
              </div>
              
              </v-col> -->
            
          </div>
        </v-col>
        <v-col cols="12">
          <div class="first" id="certification">
            <h2 class="black--text">CERTIFICATION</h2>
            <!-- Start Certification -->
            <v-col cols="12">
              <div class="child">
                <v-card class="mx-auto" width="344">

                  <v-card-title>
                    Deep Learning Training
                  </v-card-title>

                  <v-card-subtitle>
                    Gadjah Mada University & NVIDIA
                  </v-card-subtitle>

                  <v-card-actions>
                    <v-spacer></v-spacer>
                    <v-btn icon @click="show = !show">
                      <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
                    </v-btn>
                  </v-card-actions>

                  <v-expand-transition>
                    <div v-show="show">
                      <v-divider></v-divider>
                      <v-card-text>
                        <ul>
                          <li><a href="https://courses.nvidia.com/certificates/5d8589406efa48dab0931e505cb366ab/" target="_blank">Accelerating End-to-End Data Science Workflows</a></li>
                          <li><a href="https://courses.nvidia.com/certificates/50744db951cb4aae8b743a7fd0f15a49/" target="_blank">Fundamentals of Accelerated Computing with CUDA Python</a></li>
                          <li><a href="https://courses.nvidia.com/certificates/cef040a49ce34d138543c6d0f56ef643/" target="_blank">Getting Started with Deep Learning</a></li>
                        </ul>
                      </v-card-text>
                    </div>
                  </v-expand-transition>
                </v-card>
              </div>
              <div class="child">
                <v-card class="mx-auto" width="344">
                  <v-card-title>
                    Dicoding Training
                  </v-card-title>

                  <v-card-subtitle>
                    Dicoding Indonesia
                  </v-card-subtitle>

                  <v-card-actions>
                    <v-spacer></v-spacer>
                    <v-btn icon @click="show = !show">
                      <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
                    </v-btn>
                  </v-card-actions>

                  <v-expand-transition>
                    <div v-show="show">
                      <v-divider></v-divider>
                      <v-card-text>
                        <ul>
                          <li><a href="https://www.dicoding.com/certificates/0LZ0DWKLKX65" target="_blank">Belajar Membuat Augmented Reality dengan Lens Studio</a></li>
                          <li><a href="https://www.dicoding.com/certificates/JLX11JYDJX72" target="_blank">Belajar Dasar Pemrograman JavaScript</a></li>
                          <li><a href="https://www.dicoding.com/certificates/98XW6Y49LXM3" target="_blank">Cloud Practitioner Essentials (Belajar Dasar AWS Cloud)</a></li>
                        </ul>
                      </v-card-text>
                    </div>
                  </v-expand-transition>
                </v-card>
              </div>
            </v-col>
            <v-col cols="12">
              <div class="child">
                <v-card class="mx-auto" width="344">

                  <v-card-title>
                    KMMI Machine Learning
                  </v-card-title>

                  <v-card-subtitle>
                    Ciputra University & METRODATA ACADEMY
                  </v-card-subtitle>

                  <v-card-actions>
                    <v-spacer></v-spacer>
                    <v-btn icon @click="show = !show">
                      <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
                    </v-btn>
                  </v-card-actions>

                  <v-expand-transition>
                    <div v-show="show">
                      <v-divider></v-divider>
                      <v-card-text>
                        <ul>
                          <li>
                            <a href="https://drive.google.com/file/d/1r7bpR2dIjzNBsR8UUPaLLZ4i5TOLQUeH/view" target="_blank">Certification of Achievement</a>
                          </li>
                        </ul>
                      </v-card-text>
                    </div>
                  </v-expand-transition>
                </v-card>
              </div>
              <div class="child">
                <v-card class="mx-auto" width="344">

                  <v-card-title>
                    Bootcamp Data Science Batch 3
                  </v-card-title>

                  <v-card-subtitle>
                    DQLab
                  </v-card-subtitle>

                  <v-card-actions>
                    <v-spacer></v-spacer>
                    <v-btn icon @click="show = !show">
                      <v-icon>{{ show ? 'mdi-chevron-up' : 'mdi-chevron-down' }}</v-icon>
                    </v-btn>
                  </v-card-actions>

                  <v-expand-transition>
                    <div v-show="show">
                      <v-divider></v-divider>
                      <v-card-text>
                        <ul>
                          <li><a href="https://academy.dqlab.id/certificate/pdf/DQLABSQLT1CFQNBN" target="_blank">Fundamental SQL Using SELECT Statement</a></li>
                          <li><a href="https://academy.dqlab.id/certificate/pdf/DQLABINTP1TOUMTQ" target="_blank">Python Fundamental for Data Science</a></li>
                          <li><a href="https://academy.dqlab.id/certificate/pdf/DQLABINTR1SLOWFR" target="_blank">R Fundamental for Data Science</a></li>
                        </ul>
                      </v-card-text>
                    </div>
                  </v-expand-transition>
                </v-card>
              </div>
              
            </v-col>
            <!-- end -->
          </div>
        </v-col>

       <v-col cols="12">
         <div class="first" id="contact">
           <h2 class="black--text">Contact</h2>
              <a href="https://linkedin.com/in/susiana-sunjaya-1077361b5" target="_blank" >
                <img src="../assets/linkedin.png" alt="linkedin" width="80px">
              </a>
              <a href="mailto:susianasunjaya@gmail.com">
                <img src="../assets/email.png" alt="linkedin" width="80px">
              </a>
              <a href="https://github.com/susianasunjaya/" target="_blank">
                <img src="../assets/github.png" alt="linkedin" width="80px">
              </a>
                  
         </div>
       </v-col>
        
    </v-container>
    <Footer />
  </v-app>
</template>

<script>
import NavBar from "../components/NavBar.vue";
import Footer from "../components/Footer.vue";
export default {
  name: "Home",
  data: () => ({
    icons: ["mdi-facebook", "mdi-twitter", "mdi-linkedin", "mdi-instagram"],
    show: false,
    messages: [
        {
          // avatar: 'https://avatars0.githubusercontent.com/u/9064066?v=4&s=460',
          color: 'black',
          icon: 'mdi-translate',
          name: 'Mandarin Tutor',
          title: 'Elementary School and HSK 1',
          detail1:"Mengajar secara langsung (luring dan daring) bahasa Mandarin tingkat dasar dengan jumlah siswa sebanyak satu hingga tujuh siswa.",
          detail2:"Membuat soal latihan dan materi yang sesuai dengan kurikulum sekolah siswa serta menilai hasil kerja siswa.",
        },
        {
          color: 'black',
          icon: 'mdi-laptop',
          name: 'Assistant Lecturer',
          title: 'Algorithm and Programming',
          detail1:"Membuat soal unguided yang akan dikerjakan oleh mahasiswa dengan menggunakan Python sebagai bahasa pemrograman.",
          detail2:"Menilai hasil unguided dan ujian yang telah dikerjakan mahasiswa.",
        },
        {
          color: 'black',
          icon: 'mdi-laptop',
          name: 'Assistant Lecturer',
          title: 'Database System',
          detail1:"Membuat soal unguided dan soal ujian yang akan dikerjakan oleh mahasiswa dengan menggunakan Microsoft Access dan MySQL.",
          detail2:"Menilai hasil unguided dan ujian yang telah dikerjakan mahasiswa.",
          exceprt: 'New deals available, Join Today',
        },
        {
          color: 'black',
          icon: 'mdi-laptop',
          name: 'Assistant Lecturer',
          title: 'Web Programming',
          detail1:"Membuat soal unguided dan soal ujian yang akan dikerjakan oleh mahasiswa dengan menggunakan HTML, CSS, PHP, dan JavaScript.",
          detail2:"Menilai hasil unguided dan ujian yang telah dikerjakan mahasiswa.",
          // exceprt: 'New deals available, Join Today',
        },
      ],
      organizations: [
        {
          organization: 'Himpunan Mahasiswa Teknik Informatika',
          year:'2020',
          title: 'Secretary',
          color: 'pink',
        },
        {
          organization: 'Kamadhis Duta Dharma',
          year: '2020',
          title: 'Internal Division',
          color: 'pink',
        },
        {
          organization: 'Kamadhis Duta Dharma',
          year: '2021',
          title: 'Treasurer',
          color: 'pink',
        },
      ],
  }),
  components: {
    NavBar,
    Footer,
  },
};
</script>
<style scoped>

.first {
  text-align: center;
  padding: 2rem 2rem;
}

.child {
  display: inline-block;
  padding: 2rem 1rem;
  vertical-align: middle;
  text-align: left;
  margin-right: 8px;
}

.col-12.padd {
  padding: 12px 0 !important;
}


.homeprofile {
  background-image: url(../assets/zero.png);
  background-size: cover;
  background-position: center;
  height: max-content;
}

#welcome {
  font-size: 200px;
}
img{
  margin: 20px;
}

h3{
  color: rgb(234, 9, 159);
}

a:link {
  color: rgb(234, 9, 159);
}

/* visited link */
a:visited {
  color: rgb(234, 9, 159);
}

/* mouse over link */
a:hover {
  color: rgb(234, 9, 159);
}

/* selected link */
a:active {
  color: rgb(234, 9, 159);
}


</style>