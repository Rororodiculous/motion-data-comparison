<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>README - Motion Data Comparison Tool</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      max-width: 800px;
      margin: auto;
      padding: 20px;
      line-height: 1.6;
    }
    h1, h2 {
      color: #333;
    }
    code {
      background: #eee;
      padding: 2px 4px;
      border-radius: 4px;
    }
    pre {
      background: #f4f4f4;
      padding: 10px;
      overflow-x: auto;
    }
  </style>
</head>
<body>

  <h1>Motion Data Comparison Tool</h1>

  <p>This interactive web tool simulates the motion of a car undergoing <strong>constant acceleration</strong> and outputs realistic measurements from two different types of sensors:</p>
  <ul>
    <li>A <strong>position sensor</strong> (like GPS or laser tracker) with smooth, small noise</li>
    <li>An <strong>accelerometer</strong> (like a motion chip inside the car) with jittery, higher-frequency noise</li>
  </ul>
  <p>Each dataset is <strong>unique</strong> and allows students to investigate how numerical derivatives and integrals behave in noisy real-world data.</p>

  <h2>🔍 Learning Objectives</h2>
  <ul>
    <li>Compare velocity derived from <strong>position vs. acceleration</strong></li>
    <li>Understand how <strong>noise characteristics</strong> impact data interpretation</li>
    <li>Apply <strong>numerical differentiation and integration</strong> in Excel</li>
    <li>Discuss pros and cons of different sensor types in physical experiments</li>
  </ul>

  <h2>📈 Simulation Details</h2>
  <ul>
    <li>The motion follows: <code>x(t) = x₀ + v₀ * t + 0.5 * a * t²</code></li>
    <li><strong>True acceleration</strong> and <strong>initial velocity</strong> are randomly chosen each time</li>
    <li>25 time points at 0.5 s intervals</li>
    <li>
      Noise simulation:
      <ul>
        <li><strong>Position:</strong> low-frequency, < 5% deviation</li>
        <li><strong>Acceleration:</strong> jittery, ±10% deviation</li>
      </ul>
    </li>
  </ul>

  <h2>💾 Output Format (CSV)</h2>
  <pre>
Simulated Motion Data
Velocity Comparison via Derivatives and Integrals
True Acceleration: 0.927 m/s²
Initial Velocity: 1.137 m/s

Time,Position,Acceleration
0.00,0.0012,0.8942
0.50,0.3812,0.9762
...
  </pre>

  <p>Paste the output into <strong>Excel</strong> to:</p>
  <ul>
    <li>Calculate velocity from position (via difference)</li>
    <li>Calculate velocity from acceleration (via integration)</li>
    <li>Plot and compare both methods</li>
  </ul>

  <h2>📁 Recommended Folder Name</h2>
  <pre>motion-data-comparison</pre>

  <h2>🌐 Try It Live</h2>
  <p>Host on GitHub Pages and visit:</p>
  <pre>https://Rororodiculous.github.io/motion-data-comparison/</pre>
  <p>Replace <code>yourusername</code> with your GitHub username.</p>

  <h2>📚 License</h2>
  <p>MIT License — free to use for education and modification.</p>

  <hr>
  <p><em>Built to explore real-world data uncertainty in kinematics labs.</em></p>

</body>
</html>
