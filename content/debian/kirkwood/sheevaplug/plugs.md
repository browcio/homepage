---
title: Debian and Plug Computer models
nav: Plug Variants
description: Plug Variants and whether they're supported by Debian
keywords: [Debian, SheevaPlug, plug, plugs, plug computer]
---

<% content_for :right do %>
<img src = "../images/r_sheevaplug_hand.jpg" class="border" alt="SheevaPlug in my hand" width="148" height="129" />

<%= render "adsense-wideskyscaper-right" %>
<% end %>

<h1>Plug Computer models and how well they are supported in Debian</h1>

There are many different variants of the plug computer and not all variants
are supported by Debian.  This page provides an overview of different plug
computer models and describes how well they are supported by Debian.

Generally speaking, there are two classes of plug computer: development
kits and retail products.  The development kits include a debugging module
(either internally or externally) that offers access to the serial console
and to JTAG.  This debugging option is important in case something goes
wrong with the installation or operation of Debian.  Because of the
importance of the debugging module, I'm primarily planning to support
development kits.  There will also be limited support for some retail
products to which users have manually added a serial console.  However,
adding a serial console to a retail product will usually involve soldering
and no support for this process is given here.  Therefore, unless you know
how to tinker with hardware, make sure to get a development kit with a
debugging module!

<h2>Models with full support</h2>

The following models are fully supported by Debian.  Please read the <a
href = "../install">installation guide</a> if you want to install Debian.

<ul>

<li>SheevaPlug (or, more accurately, SheevaPlug Development Kit): this is
the original SheevaPlug and it's fully supported.  You can obtain this
device from <a href = "http://www.globalscaletechnologies.com/">GlobalScale
Technologies</a> in the US and from <a href =
"http://www.newit.co.uk/">NewIT</a> in Europe.</li>

<li>eSATA SheevaPlug: like the SheevaPlug, but it also offers eSATA.</li>

<li>GuruPlug (GuruPlug Server Standard and GuruPlug Server Plus): in
addition to the functionality of the SheevaPlug, the GuruPlug Server offers
wireless and Bluetooth.  The GuruPlug Server Standard offers one Ethernet
and one USB port whereas the GuruPlug Server offers two Ethernet, one
eSATA, two USB and one micro SD ports.  Make sure you get the GuruPlug
JTAG, which is sold separately.  Note that the GuruPlug has a fan.</li>

<li>KURO-SHEEVA: a plug sold in Japan that is very similar to the eSATA
SheevaPlug.  Please follow the instructions for the eSATA SheevaPlug.</li>

<li>Ionics Nimbus 100: this device is compatible with the original
SheevaPlug and is therefore supported.  However, make sure you get the
development kit rather than the retail version since the USB-based debug
connection (with access to UART and JTAG) is only included in the
development kit.  This plug is available from <a href =
"http://www.ionicsplug.com/nimbus100.html">Ionics</a>.</li>

</ul>

<h2><a id = "limited">Models with limited support</a></h2>

The following model is supported by Debian but you have to manually add a
serial console to your device in order to install Debian.  No help is given
here for adding a serial console so I suggest you buy a development kit
with debugging module if you don't know how to add a serial console.  If
you have successfully added a serial console and can interact with u-boot,
follow the <a href = "../install">installation guide</a> to install Debian.

<ul>

<li>Seagate FreeAgent DockStar: there are some external guides explaining
how to add a serial console.  See <a href =
"http://www.rudiswiki.de/wiki/DockStarSerialLink">here</a> and <a href =
"http://www.yourwarrantyisvoid.com/2010/07/21/seagate-dockstar-add-an-accessible-serial-port/">here</a>.</li>

</ul>

<h2>Models that will be supported in the future</h2>

<ul>

<li>DreamPlug: the DreamPlug will be supported in Debian wheezy (Debian
7.0) thanks to the work of Ian Campbell.</li>

</ul>

<h2>Models that may or may not be supported in the future</h2>

<ul>

<li>GuruPlug Display: this device looks interesting but is based on a
different chip than all other plugs.  While most plugs use a Marvell
Kirkwood chip, the GuruPlug Display is based on a Marvell PXA chip which we
currently don't support in Debian.  At the moment, I'm not planning to
support this model.</li>

<li>Ionics Nimbus 200, Nimbus 300, Cumulus, Stratus and Cirrus: I asked
Ionics for hardware and didn't get a reply so I'm not planning to support
these devices.  However, adding support is possible if someone wants to
work on it.  If you intend to purchase such a device, be aware that the
Nimbus and Cumulus need an external JTAG/serial module.  The Stratus and
Cirrus have an internal JTAG/serial module but <em>only</em> only the
Development Kit version.</li>

</ul>

<h2>Unsupported models without plans to support</h2>

The following devices are retail products which lack the debugging option.
They will not be supported:

<ul>

<li>CloudPlug</li>

<li>PogoPlug</li>

<li>TonidoPlug</li>

</ul>

Go back to my <a href = "..">Debian on Plug Computer</a> page.

<%= render "paypal", :desc => "Debian on Plug Computer donation" %>

<div class="bbf">
<%= render "adsense-banner-before-footer" %>
</div>
