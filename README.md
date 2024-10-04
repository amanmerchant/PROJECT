gsap.registerPlugin(ScrollTrigger);

gsap.from(".my-element", {
  opacity: 0,         // Start with the element completely transparent
  y: 100,             // Move it 100 pixels down initially
  duration: 1,        // Animation duration is 1 second
  scrollTrigger: {
    trigger: ".my-element",  // The element that triggers the animation
    start: "top 80%",        // When the top of the element reaches 80% of the viewport
  }
});
