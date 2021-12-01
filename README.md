---
 - hosts: localhost

   tasks:

    - name: Ping Windows Hosts
      action: ping
      register: hello
    - debug: msg="{hello.stdout}"
