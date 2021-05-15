<template>
  <div class="w-full">
    <div
      id="about"
      class="
        headline
        h-full
        xl:h-screen
        py-16
        md:py-64
        px-8
        flex flex-col
        md:flex-row
        bg-blue-500
        relative
      "
    >
      <Particles id="about-particles" :options="particlesConfig" />
      <div class="left w-full md:w-1/2 flex justify-center align-middle pb-16">
        <div>
          <img
            class="rounded-full object-contain"
            src="https://picsum.photos/id/238/300/300"
            alt="Image"
          />
        </div>
      </div>
      <div class="right w-full md:w-1/2 flex justify-between flex-col">
        <div>
          <div
            class="
              content
              justify-end
              border-b-8 border-white
              mb-8 mb-8
              pb-4
              -mr-8
            "
          >
            <div class="text pr-8">
              <h1 class="text-5xl sm:text-6xl md:text-8xl uppercase text-white">
                Jan Liber
              </h1>
              <h4 class="text-2xl sm:text-3xl md:text-4xl text-white">
                Web Developer
              </h4>
            </div>
          </div>
          <p class="text-white">
            I'm a 22 year old guy from Slovenia. I enjoy writing code and
            drinking coffee.
          </p>
        </div>

        <ul class="socials mt-16 flex flex-wrap">
          <li
            class="
              flex-1
              text-center
              border-8
              p-2
              border-white
              mx-2
              md:mr-6
              mb-6
              text-md
            "
          >
            <a
              href="https://github.com/ilion227"
              class="font-bold text-white text-2xl uppercase"
              target="_blank"
              >GitHub</a
            >
          </li>
          <li
            class="
              flex-1
              text-center
              border-8
              p-2
              border-white
              mx-2
              md:mr-6
              mb-6
              text-md
            "
          >
            <a
              href="https://www.linkedin.com/in/jan-liber"
              class="font-bold text-white text-2xl uppercase"
              target="_blank"
              >LinkedIn</a
            >
          </li>
          <li
            class="
              flex-1
              text-center
              border-8
              p-2
              border-white
              mx-2
              md:mr-6
              mb-6
              text-md
            "
          >
            <span class="font-bold text-white text-2xl uppercase"
              >@ilion227</span
            >
          </li>
        </ul>
      </div>
    </div>
    <div
      id="projects"
      class="
        h-full
        md:h-screen
        py-16
        md:py-64
        px-8
        flex flex-col-reverse
        md:flex-row
        bg-white
      "
    >
      <div
        class="
          left
          w-full
          md:w-1/2
          flex
          justify-center
          align-middle
          pb-16
          px-0
          md:px-8
        "
      >
        &nbsp;
      </div>
      <div class="right w-full md:w-1/2 flex justify-between flex-col">
        <div>
          <div
            class="
              content
              justify-end
              border-b-8 border-blue-500
              mb-8 mb-8
              pb-4
              -mr-8
            "
          >
            <div class="text pr-8">
              <h1
                class="
                  text-4xl
                  sm:text-5xl
                  md:text-6xl
                  lg:text-7xl
                  xl:text-8xl
                  uppercase
                  text-blue-500
                "
              >
                Projects
              </h1>
            </div>
          </div>
          <p class="text-blue-500">
            All of the projects I have created or participated on.
          </p>
        </div>
      </div>
    </div>
    <div
      id="skills"
      class="
        h-full
        md:h-screen
        py-16
        md:py-64
        px-8
        flex flex-col-reverse
        md:flex-row
        bg-green-500
      "
    >
      <div
        class="
          left
          w-full
          md:w-1/2
          flex
          justify-center
          align-middle
          pb-16
          px-0
          md:px-8
        "
      >
        <!--<div class="w-full h-full mx-auto bg-white"></div>-->
      </div>
      <div class="right w-full md:w-1/2 flex justify-between flex-col">
        <div>
          <div
            class="
              content
              justify-end
              border-b-8 border-white
              mb-8 mb-8
              pb-4
              -mr-8
            "
          >
            <div class="text pr-8">
              <h1
                class="
                  text-4xl
                  sm:text-5xl
                  md:text-6xl
                  lg:text-7xl
                  xl:text-8xl
                  uppercase
                  text-white
                "
              >
                Skills
              </h1>
            </div>
          </div>
          <p class="text-white">Skills I have in web development.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      particlesConfig: {
        particles: {
          number: { value: 240, density: { enable: true, value_area: 800 } },
          color: { value: '#ffffff' },
          shape: {
            type: 'circle',
            stroke: { width: 0, color: '#000000' },
            polygon: { nb_sides: 5 },
            image: { src: 'img/github.svg', width: 100, height: 100 },
          },
          opacity: {
            value: 1,
            random: true,
            anim: { enable: true, speed: 1, opacity_min: 0, sync: false },
          },
          size: {
            value: 3,
            random: true,
            anim: { enable: false, speed: 4, size_min: 0.3, sync: false },
          },
          line_linked: {
            enable: false,
            distance: 150,
            color: '#ffffff',
            opacity: 0.4,
            width: 1,
          },
          move: {
            enable: true,
            speed: 1,
            direction: 'none',
            random: true,
            straight: false,
            out_mode: 'out',
            bounce: false,
            attract: { enable: false, rotateX: 600, rotateY: 600 },
          },
        },
        interactivity: {
          detect_on: 'canvas',
          events: {
            onhover: { enable: true, mode: 'bubble' },
            onclick: { enable: true, mode: 'repulse' },
            resize: true,
          },
          modes: {
            grab: { distance: 400, line_linked: { opacity: 1 } },
            bubble: {
              distance: 250,
              size: 0,
              duration: 2,
              opacity: 0,
              speed: 3,
            },
            repulse: { distance: 400, duration: 0.4 },
            push: { particles_nb: 4 },
            remove: { particles_nb: 2 },
          },
        },
        detectRetina: true,
      },
    }
  },
}
</script>

<style>
* {
  font-family: 'Montserrat', sans-serif;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-family: 'Monoton', cursive;
}

#about-particles {
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  z-index: 0;
}

.left,
.right {
  z-index: 99;
}
</style>
