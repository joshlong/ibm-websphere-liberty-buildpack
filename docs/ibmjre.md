#Repackage the IBM JRE

The IBM JRE that is available on the [developerWorks Java site][] is available in a
.bin format. The buildpack, however, requires a .tgz archive. Follow these instructions to build a
.tgz archive from the .bin file.

* Upload the .bin file to a directory on your Linux machine

* Ensure that the executable bit is set on the file

```bash
sudo chmod +x ibm-java-jre-7.0-5.0-x86_64-archive.bin
```

* Start the install

```bash
./ibm-java-jre-7.0-5.0-x86_64-archive.bin
```

* Select the language

* Accept the license

* Accept the default installation location

* Once the installation is complete, execute the following command to build the .tgz archive

```bash
tar cvfz ibm-java-jre-7.0-5.0-linux-x86_64.tgz ibm-java-x86_64-70
```

  where ibm-java-jre-7.0-5.0-linux-x86_64.tgz is the name of the package that you want to build, and
  ibm-java-x86_64-70 is the name of the directory into which the JRE was installed.

[developerWorks Java site]: https://www.ibm.com/developerworks/java/jdk/