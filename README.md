# AnaEuropa
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mon Calendrier</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 20px;
        }
        #calendar {
            max-width: 800px;
            margin: 0 auto;
        }
        .media-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 10px;
            margin-top: 20px;
        }
        .media-item {
            max-width: 300px;
        }
    </style>
</head>
<body>
    <div id="calendar"></div>
    <div class="media-container">
        <img class="media-item" src="https://via.placeholder.com/300" alt="Image placeholder">
        <video class="media-item" controls>
            <source src="https://example.com/video.mp4" type="video/mp4">
            Votre navigateur ne supporte pas la balise vidéo.
        </video>
    </div>

    <script src="https://cdn.jsdelivr.net/npm/fullcalendar@5.10.2/main.min.js"></script>
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/fullcalendar@5.10.2/main.min.css">
    <script>
        document.addEventListener('DOMContentLoaded', function() {
            var calendarEl = document.getElementById('calendar');
            var calendar = new FullCalendar.Calendar(calendarEl, {
                initialView: 'dayGridMonth'
            });
            calendar.render();
        });
    </script>
</body>
</html>
