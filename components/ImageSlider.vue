<!-- <template>
  <div class="image-slider">
    <div class="slide" :style="{ backgroundImage: 'url(' + currentImage + ')' }"></div>
    <div class="controls">
      <button @click="prevImage" :disabled="currentIndex === 0">Previous</button>
      <button @click="nextImage" :disabled="currentIndex === images.length - 1">Next</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      images: [
        'public/images/fashionable-man-woman-sitting-stair 1.png',
        '/image2.jpg',
        '/image3.jpg'
        // Add more image paths as needed
      ],
      currentIndex: 0
    };
  },
  computed: {
    currentImage() {
      return this.images[this.currentIndex];
    }
  },
  methods: {
    nextImage() {
      this.currentIndex = (this.currentIndex + 1) % this.images.length;
    },
    prevImage() {
      this.currentIndex = (this.currentIndex - 1 + this.images.length) % this.images.length;
    }
  }
};
</script>

<style scoped>
.image-slider {
  width: 100%;
  max-width: 600px;
  margin: auto;
  overflow: hidden;
  position: relative;
}

.slide {
  width: 100%;
  height: 300px; /* Adjust height as per your images */
  background-size: cover;
  background-position: center;
}

.controls {
  position: absolute;
  bottom: 10px;
  left: 0;
  right: 0;
  text-align: center;
}

.controls button {
  padding: 10px 20px;
  margin: 0 10px;
  cursor: pointer;
}
</style> -->