Commands used to execute the code

Terminal 1 :  perf stat ./uds_server

Terminal 2 :  perf stat ./uds_client

Commands used to show performance counter stats syscalls

Terminal 1 :  sudo perf stat -e syscalls:sys_enter_read,syscalls:sys_enter_write,syscalls:sys_enter_accept -- ./uds_server

Terminal 2 :  sudo perf stat -e syscalls:sys_enter_read,syscalls:sys_enter_write,syscalls:sys_enter_accept -- ./uds_client

