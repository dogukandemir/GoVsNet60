# Go vs Net60 vs Net50

This repo has 3 simple api projects. `WebApplicationNet60`, `WebApplicationNet50` and `WebApplicationGo`. All projects are creating WeatherForecast array with 5 elements in it and return that array as json.

| Application         |  Port  | Local Address                          |
|---------------------|--------|----------------------------------------|
| WebApplicationNet60 |  5000  | http://localhost:5000/weatherforecast  |
| WebApplicationNet50 |  5000  | http://localhost:5000/weatherforecast  |
| WebApplicationGo    |  10000 | http://localhost:10000/weatherforecast |

## Load testing (k6s)
You'll find `net60.js`, `net50.js` and `go.js` under `LoadTests` folder.

## 100 VUs 30 sec
![GoVsNet60-100VUs-30sec](/LoadTests/GoVsNet60-100VUs-30sec.png)
![Net50-100VUs-30sec](/LoadTests/Net50-100VUs-30sec.png)
![Java-Spring-100VUs-30sec](/LoadTests/java.png)