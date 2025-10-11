# Ex.07 Restaurant Website
## Date:08-10-25

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
```

// File: GreenSpot.jsx
import { motion } from "framer-motion";
import { Button } from "@/components/ui/button";
import { Card, CardContent } from "@/components/ui/card";

export default function GreenSpot() {
  return (
    <div className="min-h-screen bg-gradient-to-br from-green-50 via-white to-emerald-50 text-gray-800 font-sans">
      {/* Header */}
      <header className="flex justify-between items-center px-6 py-5 bg-white/70 backdrop-blur-md shadow-md">
        <motion.div
          initial={{ opacity: 0, y: -10 }}
          animate={{ opacity: 1, y: 0 }}
          className="space-y-1"
          >
          <h1 className="text-3xl font-bold bg-gradient-to-r from-green-700 to-lime-500 bg-clip-text text-transparent">
            Green Spot
          </h1>
          <p className="text-sm text-gray-500">Fresh • Organic • Local — Student-friendly dining</p>
        </motion.div>
        <Button className="bg-gradient-to-r from-green-500 to-lime-400 text-white shadow-md hover:scale-105 transition-transform">
          Order Online
        </Button>
      </header>

      {/* Navigation */}
      <nav className="flex flex-wrap justify-center gap-3 mt-6">
        {["Home", "Menu", "Book a Table", "Opening Hours", "Contact"].map((tab, i) => (
          <Button
            key={i}
            className={`rounded-full px-5 py-2 text-gray-900 shadow-sm hover:scale-105 transition-transform ${
              i === 0
                ? "bg-lime-200 hover:bg-lime-300"
                : i === 1
                ? "bg-green-200 hover:bg-green-300"
                : i === 2
                ? "bg-emerald-200 hover:bg-emerald-300"
                : i === 3
                ? "bg-teal-200 hover:bg-teal-300"
                : "bg-yellow-200 hover:bg-yellow-300"
            }`}
          >
            {tab}
          </Button>
        ))}
      </nav>

      {/* Offer Banner */}
      <motion.div
        initial={{ opacity: 0 }}
        animate={{ opacity: 1 }}
        transition={{ delay: 0.4 }}
        className="text-center mt-8"
      >
        <div className="inline-block bg-green-800 text-white px-8 py-3 rounded-full font-semibold shadow-md hover:scale-105 transition-transform">
          🌿 25% Off All Healthy Bowls This Weekend!
        </div>
      </motion.div>

      {/* Content Section */}
      <section className="grid sm:grid-cols-3 gap-6 max-w-6xl mx-auto mt-12 px-6">
        {/* Card 1 */}
        <motion.div
          whileHover={{ scale: 1.03 }}
          className="bg-green-100 rounded-2xl shadow-lg overflow-hidden"
        >
          <img
            src="https://images.unsplash.com/photo-1551218808-94e220e084d2?auto=format&fit=crop&w=800&q=80"
            alt="Vegan meal"
            className="h-40 w-full object-cover"
          />
          <CardContent className="p-5">
            <h2 className="font-semibold text-lg mb-2">Our Fresh Menu</h2>
            <p className="text-sm text-gray-600 mb-3">
              Explore our organic, plant-based dishes made from locally sourced ingredients. Healthy and affordable.
            </p>
            <a href="#" className="text-green-700 font-medium hover:underline">
              See our menu →
            </a>
          </CardContent>
        </motion.div>

        {/* Card 2 */}
        <motion.div
          whileHover={{ scale: 1.03 }}
          className="bg-emerald-100 rounded-2xl shadow-lg overflow-hidden"
        >
          <img
            src="https://images.unsplash.com/photo-1568605114967-8130f3a36994?auto=format&fit=crop&w=800&q=80"
            alt="Restaurant interior"
            className="h-40 w-full object-cover"
          />
          <CardContent className="p-5">
            <h2 className="font-semibold text-lg mb-2">Book a Table</h2>
            <p className="text-sm text-gray-600 mb-3">
              Reserve your spot for a relaxing, green dining experience. Perfect for groups and study nights.
            </p>
            <a href="#" className="text-emerald-700 font-medium hover:underline">
              Book now →
            </a>
          </CardContent>
        </motion.div>

        {/* Card 3 */}
        <motion.div
          whileHover={{ scale: 1.03 }}
          className="bg-teal-100 rounded-2xl shadow-lg overflow-hidden"
        >
          <img
            src="https://images.unsplash.com/photo-1504674900247-0877df9cc836?auto=format&fit=crop&w=800&q=80"
            alt="Chef preparing salad"
            className="h-40 w-full object-cover"
          />
          <CardContent className="p-5">
            <h2 className="font-semibold text-lg mb-2">Opening Hours</h2>
            <p className="text-sm text-gray-600 mb-3">
              Mon–Fri: 11am–10pm • Sat: 12pm–11pm • Sun: 2pm–9pm
            </p>
            <a href="#" className="text-teal-700 font-medium hover:underline">
              Contact & directions →
            </a>
          </CardContent>
        </motion.div>
      </section>

      {/* Footer */}
      <footer className="text-center text-gray-500 text-sm mt-12 pb-6">
        Designed with 🌱 love • Green Spot — healthy dining for everyone
      </footer>
    </div>
  );
}

```

## OUTPUT:


![alt text](<Screenshot 2025-10-11 142115.png>)


## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
