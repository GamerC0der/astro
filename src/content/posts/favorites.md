---
title: My Favorites of 2025
description: A list of my favorite things from 2025!
pubDate: Dec 23 2025
---

I've used a lot of tools in 2025, and I wanted to share some of my favorites!<br><br>
Favorite Editor

<canvas id="editorChart" width="400" height="400" style="max-width: 100%;"></canvas>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/gh/devicons/devicon@v2.15.1/devicon.min.css">
<script>
document.addEventListener('DOMContentLoaded', function() {
  const ctx = document.getElementById('editorChart').getContext('2d');
  new Chart(ctx, {
    type: 'bar',
    data: {
      labels: ['Cursor', 'Visual Studio Code', 'Windsurf', 'Visual Studio'],
      datasets: [{
        label: 'Hours Used',
        data: [531, 17, 4, 3],
        backgroundColor: [
          '#4CAF50',
          '#2196F3',
          '#FF9800',
          '#9C27B0'
        ],
        borderColor: [
          '#45a049',
          '#1976D2',
          '#F57C00',
          '#7B1FA2'
        ],
        borderWidth: 1
      }]
    },
    options: {
      responsive: true,
      maintainAspectRatio: false,
      scales: {
        y: {
          beginAtZero: true,
          title: {
            display: true,
            text: 'Hours'
          }
        },
        x: {
          title: {
            display: false
          }
        }
      },
      plugins: {
        legend: {
          display: false
        },
        tooltip: {
          callbacks: {
            label: function(context) {
              return context.parsed.y + ' hours';
            }
          }
        }
      }
    }
  });
});
</script>

<div style="text-align: center; margin: 20px 0; font-weight: bold;">Winner: Cursor</div>

Favorite Models

<div style="background-color: #1a1a1a; padding: 20px; border-radius: 8px; font-family: system-ui, -apple-system, sans-serif;">
  <div class="model-item" style="display: flex; align-items: center; padding: 12px 0; border-bottom: 1px solid #2a2a2a; opacity: 0; transform: translateY(20px); transition: all 0.5s ease;">
    <span style="color: #888; font-size: 14px; width: 30px; flex-shrink: 0;">1</span>
    <span style="color: white; font-size: 18px; font-weight: 500; flex: 1;">Grok Code Fast 1</span>
  </div>
  <div class="model-item" style="display: flex; align-items: center; padding: 12px 0; border-bottom: 1px solid #2a2a2a; opacity: 0; transform: translateY(20px); transition: all 0.5s ease;">
    <span style="color: #888; font-size: 14px; width: 30px; flex-shrink: 0;">2</span>
    <span style="color: white; font-size: 18px; font-weight: 500; flex: 1;">Auto</span>
  </div>
  <div class="model-item" style="display: flex; align-items: center; padding: 12px 0; border-bottom: 1px solid #2a2a2a; opacity: 0; transform: translateY(20px); transition: all 0.5s ease;">
    <span style="color: #888; font-size: 14px; width: 30px; flex-shrink: 0;">3</span>
    <span style="color: white; font-size: 18px; font-weight: 500; flex: 1;">Code Supernova</span>
  </div>
  <div class="model-item" style="display: flex; align-items: center; padding: 12px 0; border-bottom: 1px solid #2a2a2a; opacity: 0; transform: translateY(20px); transition: all 0.5s ease;">
    <span style="color: #888; font-size: 14px; width: 30px; flex-shrink: 0;">4</span>
    <span style="color: white; font-size: 18px; font-weight: 500; flex: 1;">GPT 4.1</span>
  </div>
  <div class="model-item" style="display: flex; align-items: center; padding: 12px 0; border-bottom: 1px solid #2a2a2a; opacity: 0; transform: translateY(20px); transition: all 0.5s ease;">
    <span style="color: #888; font-size: 14px; width: 30px; flex-shrink: 0;">5</span>
    <span style="color: white; font-size: 18px; font-weight: 500; flex: 1;">Claude 4 Sonnet</span>
  </div>
  <div class="model-item" style="display: flex; align-items: center; padding: 12px 0; opacity: 0; transform: translateY(20px); transition: all 0.5s ease;">
    <span style="color: #888; font-size: 14px; width: 30px; flex-shrink: 0;">6</span>
    <span style="color: white; font-size: 18px; font-weight: 500; flex: 1;">GPT 5</span>
  </div>
</div>

<p style="margin-top: 20px; color: #888; font-size: 14px;">I typically run Grok Code Fast 1 with at least 2 work trees on Cursor but sometimes even 4 for quick, cheap, simple edits.</p>

<br>
Most Used Language

<div id="languagePercentage" style="text-align: center; margin: 20px 0; font-weight: bold; font-size: 24px;"><i class="devicon-typescript-plain" style="margin-right: 10px;"></i>Typescript (<span id="percentageText">0</span>%)</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const percentageElement = document.getElementById('percentageText');
  let currentPercentage = 0;
  const targetPercentage = 36;
  const duration = 1000;
  const increment = targetPercentage / (duration / 50);

  const timer = setInterval(() => {
    currentPercentage += increment;
    if (currentPercentage >= targetPercentage) {
      currentPercentage = targetPercentage;
      clearInterval(timer);
    }
    percentageElement.textContent = Math.round(currentPercentage);
  }, 50);

  const modelItems = document.querySelectorAll('.model-item');
  modelItems.forEach((item, index) => {
    setTimeout(() => {
      item.style.opacity = '1';
      item.style.transform = 'translateY(0)';
    }, index * 100);
  });
});
</script>

<p style="text-align: center; color: #666; font-size: 16px;">I primarily make frontends in NextJS and React, so .ts / .tsx is a big part of what I do.</p>

<hr style="border: none; height: 2px; background: linear-gradient(to right, transparent, #333, transparent); margin: 30px 0;">

<img src="/src/content/posts/image.png" alt="Image" style="display: block; margin: 0 auto 20px auto; max-width: 100%; height: auto; border-radius: 1%;">

<div style="text-align: center; margin: 40px 0;">
  <div style="font-size: 2em; font-weight: bold;">
    Over 1800 commits yearly.
  </div>
  <a href="https://github.com/gamerc0der" target="_blank" style="text-decoration: none; color: inherit;">
    <i class="devicon-github-plain" style="font-size: 3em; margin-top: 10px; cursor: pointer;"></i>
  </a>
</div>

Most Used OS

<canvas id="osChart" width="300" height="300" style="max-width: 100%; margin: 20px auto; display: block;"></canvas>

<div id="osMessage" style="text-align: center; margin: 20px 0; font-style: italic; color: #666;"></div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const osCtx = document.getElementById('osChart').getContext('2d');
  new Chart(osCtx, {
    type: 'pie',
    data: {
      labels: ['MacOS', 'Windows', 'Linux'],
      datasets: [{
        data: [82, 16, 2],
        backgroundColor: [
          '#C0C0C0',
          '#0078D4',
          '#4CAF50'
        ],
        borderColor: [
          '#A0A0A0',
          '#005A9E',
          '#388E3C'
        ],
        borderWidth: 2
      }]
    },
    options: {
      responsive: false,
      plugins: {
        legend: {
          position: 'bottom',
          labels: {
            padding: 20,
            usePointStyle: true
          }
        },
        tooltip: {
          callbacks: {
            label: function(context) {
              return context.label + ': ' + context.parsed + '%';
            }
          }
        }
      }
    }
  });

  const osMessage = document.getElementById('osMessage');
  const userAgent = navigator.userAgent || navigator.platform;
  let userOS = 'Unknown';

  if (userAgent.indexOf('Mac') !== -1) {
    userOS = 'MacOS';
  } else if (userAgent.indexOf('Win') !== -1) {
    userOS = 'Windows';
  } else if (userAgent.indexOf('Linux') !== -1) {
    userOS = 'Linux';
  }

  if (userOS === 'MacOS') {
    osMessage.textContent = 'I see you use MacOS too!';
  } else {
    osMessage.textContent = `I see you're on ${userOS} but I'm on MacOS!`;
  }
});
</script>

<style>
  body {
    margin-bottom: 10vh;
    padding-bottom: 20px;
  }
</style>

<div style="position: fixed; bottom: 20px; left: 50%; transform: translateX(-50%); z-index: 1000;">
  <button onclick="window.location.href='/'" style="background-color: transparent; color: white; border: 2px solid white; padding: 12px 24px; border-radius: 6px; font-size: 16px; cursor: pointer;">Back</button>
</div>