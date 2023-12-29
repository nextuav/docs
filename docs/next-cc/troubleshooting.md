---
sidebar_position: 9
---

# Troubleshooting

### What to do if NextCC is not turning on?

- Check the power supply with a multimeter. It should be 5V with maximum current of 2A.

- Check the LEDs on the NextCC board. The power LED should be continuously on and the others should blink from time to
  time

### What to do if telemetry data is not coming to the GCS?

- If the telemetry air unit is powered using NextCC, ensure that the air unit is getting the proper power supply as
  listed by the telemetry manufacturer. NextCC's `Telem` port can supply 5V. If the power issue still persists, power
  the telemetry air unit separately.

- Ensure that the `Telem` port of the NextCC is connected to the Telemetry air unit’s UART Port and the `FCU` port of
  the NextCC is connected to the Pixhawk's telemetry port.

- Check the [Dashboard Home](/next-cc/dashboard-home.md) after connecting the Pixhawk to the NextCC. If the `Autopilot`
  section shows `N/A` then check the Pixhawk connections with the NextCC.

- Verify that the baud rate of the telemetry device, the NextCC, and the GCS are the same. The default baud rate is
  **57600**.

- Ensure that the telemetry port of the Pixhawk is configured with **MAVLink 2** enabled.

### The telemetry data is available on the GCS but the drone is not coming online. How to debug this?

- Check the SIM card orientation in the NextCC board. Refer the [Hardware Setup](/next-cc/getting-started/hardware-setup.md).

- Ensure that the network antennas have been connected to the `main` and `div` ports of the cellular module.

- The SIM card should have a valid recharge plan to access the internet.

- For a new SIM card, insert it in your mobile and check whether the internet is working properly and then insert the
  card in NextCC.

- If the SIM card is not inserted or inserted in the wrong orientation, in dashboard it will show the connectivity
  status as `Failed`.

- If the network antennas are not connected properly in the cellular module, in dashboard it will show the connectivity
  status as `Searching`.

- Check the connection status in NextCC dashboard's [Cellular Connectivity](/next-cc/connectivity/cellular.md) page. If
  the `Connection Status` is `Connecting` wait for a few minutes. If the status does not change or the status is
  `Connected` but the drone is still not online, try a different SIM. Contact NextUAV for support, if the problem
  persists.

### What to do if the flow meter is not working?

* Check the flow meter settings in the [Agriculture](/next-cc/agriculture.md) setup page of the NextCC dashboard.

* Check the flow meter connection with the NextCC.

### The NextCC shows that the drone is tampered, but the tamper switch is not resetting through the NextCC dashboard. What may be going wrong?

* Check the connection of the tamper switch and tamper module. 

* Check the connection of the tamper module and the NextCC.
  
* Check the cell voltage of the tamper module. Replace the cell if its below **2.5V**.
