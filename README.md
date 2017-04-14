# systemtap-practice
systemtap practice

![image](Screenshots/smileytap.svg)

## INSTALL
* CentOS
  ```
  curl https://raw.githubusercontent.com/WALL-E/static/master/setup/redhat/install_systemtap|bash
  ```

## TEST
```
# test stap
stap -V

# test kernel-debuginfo
stap -L 'kernel.function("printk")'

# test glibc-debuginfo
stap -L 'process("/lib64/libc.so.6").function("malloc")'
```

## Community Resources and Tools

* https://github.com/openresty/openresty-systemtap-toolkit

  ![image](Screenshots/tcp-accept-queue.png)

* https://github.com/youzan/systemtap-toolkit
