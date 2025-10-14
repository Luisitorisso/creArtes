// Mobile Navigation Toggle
const navToggle = document.getElementById("navToggle")
const navMenu = document.getElementById("navMenu")

navToggle.addEventListener("click", () => {
  navMenu.classList.toggle("active")
})

// Close mobile menu when clicking on a link
const navLinks = document.querySelectorAll(".nav-link")
navLinks.forEach((link) => {
  link.addEventListener("click", () => {
    navMenu.classList.remove("active")
  })
})

// Smooth scroll for anchor links
document.querySelectorAll('a[href^="#"]').forEach((anchor) => {
  anchor.addEventListener("click", function (e) {
    e.preventDefault()
    const target = document.querySelector(this.getAttribute("href"))
    if (target) {
      target.scrollIntoView({
        behavior: "smooth",
        block: "start",
      })
    }
  })
})

// Header scroll effect
let lastScroll = 0
const header = document.querySelector(".header")

window.addEventListener("scroll", () => {
  const currentScroll = window.pageYOffset

  if (currentScroll <= 0) {
    header.style.boxShadow = "0 4px 6px -1px rgba(0, 0, 0, 0.1)"
  } else {
    header.style.boxShadow = "0 10px 15px -3px rgba(0, 0, 0, 0.1)"
  }

  lastScroll = currentScroll
})

// Form Validation and Submission
const contactForm = document.getElementById("contactForm")
const formSuccess = document.getElementById("formSuccess")

contactForm.addEventListener("submit", async (e) => {
  e.preventDefault()

  // Get form data
  const formData = {
    nombre: document.getElementById("nombre").value,
    email: document.getElementById("email").value,
    telefono: document.getElementById("telefono").value,
    empresa: document.getElementById("empresa").value,
    servicio: document.getElementById("servicio").value,
    mensaje: document.getElementById("mensaje").value,
  }

  // Basic validation
  if (!formData.nombre || !formData.email || !formData.telefono || !formData.servicio || !formData.mensaje) {
    alert("Por favor completa todos los campos obligatorios.")
    return
  }

  // Email validation
  const emailRegex = /^[^\s@]+@[^\s@]+\.[^\s@]+$/
  if (!emailRegex.test(formData.email)) {
    alert("Por favor ingresa un correo electrónico válido.")
    return
  }

  // Log form data (in production, this would be sent to a server)
  console.log("[v0] Form submitted with data:", formData)

  // Show success message
  contactForm.style.display = "none"
  formSuccess.style.display = "block"

  // Optional: Send to WhatsApp
  const whatsappMessage = `Hola! Me gustaría solicitar información sobre ${formData.servicio}. Mi nombre es ${formData.nombre}, mi email es ${formData.email} y mi teléfono es ${formData.telefono}. ${formData.mensaje}`
  const whatsappUrl = `https://wa.me/50712345678?text=${encodeURIComponent(whatsappMessage)}`

  // Uncomment to auto-redirect to WhatsApp after 2 seconds
  // setTimeout(() => {
  //     window.open(whatsappUrl, '_blank');
  // }, 2000);
})

// Intersection Observer for animations
const observerOptions = {
  threshold: 0.1,
  rootMargin: "0px 0px -50px 0px",
}

const observer = new IntersectionObserver((entries) => {
  entries.forEach((entry) => {
    if (entry.isIntersecting) {
      entry.target.style.opacity = "1"
      entry.target.style.transform = "translateY(0)"
    }
  })
}, observerOptions)

// Observe all cards and sections
document
  .querySelectorAll(".problem-card, .service-card, .portfolio-item, .benefit-card, .testimonial-card")
  .forEach((el) => {
    el.style.opacity = "0"
    el.style.transform = "translateY(20px)"
    el.style.transition = "opacity 0.6s ease, transform 0.6s ease"
    observer.observe(el)
  })

// Portfolio hover effect enhancement
const portfolioItems = document.querySelectorAll(".portfolio-item")
portfolioItems.forEach((item) => {
  item.addEventListener("mouseenter", () => {
    console.log("[v0] Portfolio item hovered")
  })
})

// Track CTA button clicks
const ctaButtons = document.querySelectorAll(".btn-primary")
ctaButtons.forEach((button) => {
  button.addEventListener("click", () => {
    console.log("[v0] CTA button clicked:", button.textContent)
  })
})
