# DevOps Hackathon - Đề 005: Quản lý nhân sự (HRM)



## 5: Tường lửa UFW
root@azvps-dynamic:~# sudo ufw default deny incoming
Default incoming policy changed to 'deny'
(be sure to update your rules accordingly)
root@azvps-dynamic:~# sudo ufw default allow outgoing
Default outgoing policy changed to 'allow'
(be sure to update your rules accordingly)
root@azvps-dynamic:~# ufw allow 22/tcp
Rules updated
Rules updated (v6)
root@azvps-dynamic:~# ufw allow 80/tcp
Rules updated
Rules updated (v6)
root@azvps-dynamic:~# ufw allow 8080/tcp
Rules updated
Rules updated (v6)
root@azvps-dynamic:~# ufw enable
Command may disrupt existing ssh connections. Proceed with operation (y|n)? Y
Firewall is active and enabled on system startup
root@azvps-dynamic:~# sudo ufw status verbose
Status: active
Logging: on (low)
Default: deny (incoming), allow (outgoing), disabled (routed)
New profiles: skip

To                         Action      From
--                         ------      ----
22/tcp                     ALLOW IN    Anywhere
80/tcp                     ALLOW IN    Anywhere
8080/tcp                   ALLOW IN    Anywhere
22/tcp (v6)                ALLOW IN    Anywhere (v6)
80/tcp (v6)                ALLOW IN    Anywhere (v6)
8080/tcp (v6)              ALLOW IN    Anywhere (v6)

root@azvps-dynamic:~#
