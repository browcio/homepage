---
title: Status of D-Link DNS-323 support
nav: Status
description: Status of D-Link DNS-323 support in Debian
keywords: [Debian, D-Link, DNS-323, Conceptronic, CH3SNAS, support, status]
---

<% content_for :right do %>
<img src = "../images/r_ch3snas_front.jpg" class="border" alt="Conceptronic CH3SNAS from the front" width="148" height="146" />

<%= render "adsense-wideskyscaper-right" %>
<% end %>

<h1>Status of D-Link DNS-323 support</h1>

The D-Link DNS-323 is based on a Marvell Orion System on a Chip.  Marvell
has done a lot of work in the last few months to get support for the Orion
platform into the mainline kernel and they continue to work on getting this
platform fully supported.  However, since this is an ongoing effort, some
features of the Orion platform are currently not as well supported as in
the original Marvell LSP (Linux Support Package) used by D-Link.  Please
take this into account before deciding whether you want to install Debian,
especially if you have specific requirements (e.g. related to performance).

The table below shows how well different components of the D-Link DNS-323
are supported by Debian:

<table style="border-style: none" border="1" cellpadding="5">

<tr style="background-color: #E0E0FF">
<td>Component</td>
<td>Comment</td>
</tr>

<tr>
<td style="color: white; background-color: #00AA00">Debian</td>
<td>Debian installer works well</td>
</tr>

<tr>
<td style="color: white; background-color: #00AA00">CPU</td>
<td>Supported in mainline and Debian kernel since 2.6.25</td>
</tr>

<tr>
<td style="color: white; background-color: #00AA00">DNS-323 kernel</td>
<td>Supported in mainline and Debian kernel since 2.6.25 (revision A1).
The revision B2 is supported in the Debian kernel since 2.6.26 and in
the mainline kernel since 2.6.29</td>
</tr>

<tr>
<td style="color: white; background-color: #00AA00">SATA</td>
<td>Supported in the kernel by the `sata_mv` module.</td>
</tr>

<tr>
<td style="color: white; background-color: #00AA00">Ethernet</td>
<td>Supported in the kernel by the `mv643xx` module</td>
</tr>

<tr>
<td style="color: white; background-color: #00AA00">USB</td>
<td>Supported in the kernel since 2.6.25</td>
</tr>

<tr>
<td style="color: white; background-color: #00AA00">RTC</td>
<td>Supported in the kernel by the `rtc-m41t80` module.</td>
</tr>

<tr>
<td style="color: white; background-color: #00AA00">LEDs</td>
<td>Supported in the kernel</td>
</tr>

<tr>
<td style="color: white; background-color: #00AA00">Fan</td>
<td>Supported.</td>
</tr>

<tr>
<td style="color: white; background-color: #00AA00">Temperature sensor</td>
<td>Supported.</td>
</tr>

<tr>
<td style="color: black; background-color: #FFFF00">Crypto engine</td>
<td>Initial support in 2.6.32</td>
</tr>

</table>

<div class="bbf">
<%= render "adsense-banner-before-footer" %>
</div>
