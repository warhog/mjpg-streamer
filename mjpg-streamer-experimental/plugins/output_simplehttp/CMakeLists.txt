
add_definitions(-D_GNU_SOURCE)

MJPG_STREAMER_PLUGIN_OPTION(output_simplehttp "Simple HTTP server output plugin")
MJPG_STREAMER_PLUGIN_COMPILE(output_simplehttp simplehttpd.c output_simplehttp.c)
