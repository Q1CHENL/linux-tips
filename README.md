# Linux Tips

Things I learnt using Linux

## Commands

### `systemctl` (usually run with `sudo`)

Control the systemd system and service manager.

Important usages:

`sudo systemctl status/enable/disable/start/stop <service>`

- `status`: provides detailed information about the service, including whether it is running, stopped, enabled, or disabled, as well as recent logs related to the service.

- `enable`: configures a service to start automatically when the system boots up. It doesn't start the service immediately but ensures it will start on the next boot.

- `disable`: This command prevents a service from starting automatically at boot time. It doesn't stop a currently running service but ensures it won't start on the next boot.

- `start`: starts the service immediately. The service will run until it's stopped or the system is rebooted. It does not make the service enabled.

- `stop`: stops a running service immediately. The service will no longer run until it is started again. It does not make the service disabled.

- `<service>`
  - `firewalld`
  - `resolved`
  - `NetworkManager`
  - `systemd-resolved`
  - `sshd`
  - `dockerd`
