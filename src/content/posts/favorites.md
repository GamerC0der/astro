---
title: My Favorites of 2025
description: A list of my favorite things from 2025!
pubDate: Dec 23 2025
---

I've used a lot of tools in 2025, and I wanted to share some of my favorites!<br><br>
Favorite Editor

<canvas id="editorChart" width="400" height="400" style="max-width: 100%;"></canvas>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
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