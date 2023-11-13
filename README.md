# Apache Installation Tutorial

This tutorial provides step-by-step instructions on how to install Apache on your system.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Firewall Configuration](#firewall-configuration)
- [Accessing the Web Server in a Browser](#accessing-the-web-server-in-a-browser)
- [Remote Access to Ubuntu Server](#remote-access-to-ubuntu-server)

## Introduction

Apache HTTP Server, commonly referred to as Apache, is a widely used open-source web server. This tutorial will guide you through the process of installing Apache on your system.

## Installation

1. **Update Package Repository:**
    ```bash
    sudo apt update
    ```

2. **Upgrade Packages:**
    ```bash
    sudo apt upgrade -y
    ```

3. **Install Apache:**
    ```bash
    sudo apt install apache2 -y
    ```

## Firewall Configuration

1. **List UFW Applications:**
    ```bash
    sudo ufw app list
    ```

2. **Allow Apache Through Firewall:**
    ```bash
    sudo ufw allow 'Apache'
    ```

3. **Enable UFW:**
    ```bash
    sudo ufw enable
    ```

4. **Check UFW Status:**
    ```bash
    sudo ufw status
    ```

5. **Check Apache Status:**
    ```bash
    sudo systemctl status apache2
    ```

## Accessing the Web Server in a Browser

1. **Check the IP Address:**
    ```bash
    hostname -I
    ```

2. **Open a Browser:**
    Open a browser on your host machine.

3. **Enter the IP Address:**
    Enter the IP address of your virtual machine in your host machine's browser. The default Apache2 page should appear.
   ![Apache2](https://github.com/NauvalPerdana/Apache2/blob/main/Apache2.png)

## Remote Access to Ubuntu Server

### Command Prompt

1. **Open Command Prompt:**
    Open Command Prompt on the host machine.

2. **SSH into the Server:**
    ```bash
    ssh username@ip.address
    ```
    Replace "username" with your Ubuntu server username and "ip.address" with your Ubuntu server's IP address.

3. **Log In:**
    Type 'yes,' then log in by entering your Ubuntu server username and password.

### PuTTY

1. **Open PuTTY:**
    Open PuTTY on your host machine.

2. **Enter IP Address:**
    Enter your IP address, then click Open.

3. **Accept Connection:**
    Click Accept.

4. **Log In:**
    Log in by entering your Ubuntu server username and password.

### Ubuntu Desktop

1. **Open Ubuntu Desktop in VirtualBox:**
    Open Ubuntu Desktop in VirtualBox.

2. **Open Terminal:**
    Open Terminal in Ubuntu Desktop.

3. **SSH into the Server:**
    ```bash
    ssh username@ip.address
    ```
    Replace "username" with your Ubuntu server username and "ip.address" with your Ubuntu server's IP address. Type 'yes' and log in by entering your Ubuntu server password.
