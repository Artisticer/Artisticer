- 👋 Hi, I’m @Artisticer
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
Artisticer/Artisticer is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
---><?php
/**
 * Plugin Name: Computer Vision Plugin
 * Description: A simple WordPress plugin for computer vision using TensorFlow.js.
 * Version: 1.0
 * Author: Your Name
 */

// Enqueue JavaScript file for computer vision
function enqueue_computer_vision_script() {
    wp_enqueue_script('computer-vision-script', plugin_dir_url(__FILE__) . 'computer-vision-script.js', array('jquery'), '1.0', true);
}
add_action('wp_enqueue_scripts', 'enqueue_computer_vision_script');
