<script>
export default {
    data() {
        return {
            scrollY: 0
        }
    },
    computed: {
        shouldBackgroundNav() {
            return this.scrollY > 50;
        }
    },
    mounted() {
        window.addEventListener('scroll', (e) => {
            this.scrollY = window.scrollY;
        });
    }
}
</script>
