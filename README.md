# Frida SSL-Pinning Bypass Script

Frida SSL-pinning bypass script is a script written in the Frida tool that enables an attacker to bypass SSL certificate pinning, which is a security feature designed to prevent man-in-the-middle (MitM) attacks. SSL pinning is a technique used by mobile applications to ensure that only trusted SSL certificates are used during HTTPS communication with the application's backend server.

The Frida SSL-pinning bypass script works by hooking into the mobile application's code and intercepting the SSL traffic. It then replaces the expected SSL certificate with a custom one, effectively bypassing the SSL pinning mechanism. This allows an attacker to intercept and view the encrypted traffic between the mobile application and the backend server.

It is important to note that SSL pinning is an important security feature that helps protect against MitM attacks, and bypassing it can expose sensitive user data. As such, the Frida SSL-pinning bypass script is often used by security researchers and penetration testers to test the security of mobile applications and identify vulnerabilities that could be exploited by attackers. However, it should never be used for malicious purposes

## Pre requisites

Ensure you have [frida-tools](https://pypi.org/project/frida-tools/) installed on your computer.


## Usage

```python

#Clone git repository
git clone https://github.com/Benson306/SSL-Bypass-Script

#Get into Directory
cd SSL-Bypass-Script

#Run script to potential Victim
frida -U -f ssl.js
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first
to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License

[MIT](https://choosealicense.com/licenses/mit/)