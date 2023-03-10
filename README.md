# Weather Forecast Bot ⛅🤖
A Python-based [**Discord**](https://discord.com/) bot running on a Docker container to provide weather forecast information.

> <img src="https://user-images.githubusercontent.com/47757441/213523762-dee27ec8-d0c8-42cb-baef-0176e33f02f9.png" width="480">

### Setting up the Docker environment
1. Install [**Docker**](https://www.docker.com/products/docker-desktop/).
2. Modify the [Dockerfile](Dockerfile) and replace `YOUR_BOT_TOKEN` with a valid token provided by the [Discord Developer Portal](https://discord.com/developers/docs/intro).
3. Build the docker image. A build’s context is the set of files located in the specified `PATH`:
  ```sh
  $ docker build -t IMAGE PATH
  ```
4. Run the robot on a new container. The `docker run` command will first create a writeable container layer over the specified `IMAGE`, and then starts it using the specified command:
  ```sh
  $ docker run IMAGE
  ⋮
  WeatherBot#0000 is now running!
  ```

## Discord commands
(Work in progress)
|Command|Description|
|---|---|
|`!weather/country/COUNTRY_NAME`|Provides the current temperature in `COUNTRY_NAME`, in degrees Celsius.|
|`!help`|Provides information on built-in commands.|

## References
- [Weather Forecast API](https://open-meteo.com/en/docs#api-documentation)
- [discord.py API](https://discordpy.readthedocs.io/en/stable/api.html)
