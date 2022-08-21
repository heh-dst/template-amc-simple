# qcm-template
Multiple-choice questions template.

Works with http://auto-multiple-choice.net.

To use it:
1. Start an X11 server on your Docker host (like [VcXSrv](https://sourceforge.net/projects/vcxsrv/)) and allow incoming connections.
2. In your Docker container, set the DISPLAY environment variable to your Docker host IP address + `:0.0`
   ```sh
   export DISPLAY=172.30.160.1:0.0
   ```
3. In your Docker container, launch AMC
   ```sh
   auto-multiple-choice
   ```

# Related work

This template works along with the [froland/auto-multiple-choice](https://github.com/froland/auto-multiple-choice) public Docker image.
