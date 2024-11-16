# add-to-calendar
Dropdown button that allows people to quickly add events to their calendar 

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Add to Calendar</title>
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Kelly+Slab&display=swap');

    body {
      font-family: 'Kelly Slab', cursive;
      margin: 20px;
      font-size: 18px;
    }
    .dropdown {
      position: relative;
      display: inline-block;
    }
    .dropdown button {
      background-color: #007bff;
      color: white;
      padding: 10px 15px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      font-family: 'Kelly Slab', cursive;
      font-size: 18px;
    }
    .dropdown button:hover {
      background-color: #0056b3;
    }
    .dropdown-content {
      display: none;
      position: absolute;
      background-color: white;
      box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
      border-radius: 5px;
      z-index: 1;
      overflow: hidden;
      min-width: 200px;
    }
    .dropdown-content a {
      display: block;
      padding: 10px;
      color: #333;
      text-decoration: none;
      border-bottom: 1px solid #f1f1f1;
      font-family: 'Kelly Slab', cursive;
      font-size: 18px;
    }
    .dropdown-content a:last-child {
      border-bottom: none;
    }
    .dropdown-content a:hover {
      background-color: #f1f1f1;
    }
    .dropdown:hover .dropdown-content {
      display: block;
    }
  </style>
</head>
<body>
  <div class="dropdown">
    <button>Add to Calendar</button>
    <div class="dropdown-content">
      <a href="https://calendar.google.com/calendar/render?action=TEMPLATE&text=Bruzze+Brewing&details=&location=Bruzze+Brewing+170+Scott+Rd+suite+2,+Eatonton,+GA+31024,+USA" target="_blank">
        Google Calendar
      </a>
      <a href="https://calendar.yahoo.com/?v=60&title=Bruzze+Brewing&desc=&in_loc=Bruzze+Brewing+170+Scott+Rd+suite+2,+Eatonton,+GA+31024,+USA" target="_blank">
        Yahoo Calendar
      </a>
      <a href="https://outlook.live.com/owa/?path=/calendar/action/compose&rru=addevent&subject=Bruzze+Brewing&location=Bruzze+Brewing+170+Scott+Rd+suite+2,+Eatonton,+GA+31024,+USA" target="_blank">
        Outlook.com
      </a>
      <a href="https://outlook.office.com/calendar/0/deeplink/compose?subject=Bruzze+Brewing&location=Bruzze+Brewing+170+Scott+Rd+suite+2,+Eatonton,+GA+31024,+USA" target="_blank">
        Outlook
      </a>
      <a href="data:text/calendar;charset=utf8,BEGIN:VCALENDAR%0AVERSION:2.0%0ABEGIN:VEVENT%0ASUMMARY:Bruzze+Brewing%0ALOCATION:Bruzze+Brewing+170+Scott+Rd+suite+2,+Eatonton,+GA+31024,+USA%0AEND:VEVENT%0AEND:VCALENDAR" target="_blank">
        iCalendar
      </a>
    </div>
  </div>
</body>
</html>
