![[Pasted image 20250208140022.png]]

Ever wonder why when you trying to download files from torrent but all you get is bytes of download speed, that's your ISP that throttle the torrent speed. but how to bypass that throttle? well you gonna think of using VPN, but you need to buy VPN subscription that gonna cost $ for you, right? what if you can bypass that throttle without using VPN and for free. here (**how to**) blog gonna guide you on how to bypass ISP torrent throttle.

## Torrenting Software
the first thing you need is torrenting software, there are a lot of torrenting software that you can use, but one of my favorite is qbittorent, its free no ads like uTorrent, but the UI is kinda old looking but what you need is function not looks :D but its your choices based on what you're comfortable with. but for this (**HOW TO**) ill be using qBittorent, but here are the top 3 torrenting software:
- [qBittorrent](https://www.qbittorrent.org/)
- [uTorrent](https://www.utorrent.com/)
- [bittorrent](https://www.bittorrent.com/)

## Torrent Tracker
Torrent Tracker? 
> *A **torrent tracker** is a specialized server that helps coordinate the distribution of files in a BitTorrent network. It keeps track of peers (users) sharing a specific file and helps them find each other to facilitate faster and more efficient file transfers.* - chatgpt

so what it means is it provide you peer lists and information based on the file that you want to download, by default your torrenting software already have tracker but adding more tracker will boost and speed up your peer discovery. so your ISP could be blocking the default tracker but not the other trackers that available, sometimes tracker can be use for finding more peers for files that have less seed.

Here the tips for you about torrenting, the more seeds the file have the more peers you able to connect and fast to download, but the less seed the file is will make the downloading slow.

## Adding Additional Torrent Tracker
There are people who create lists of available trackers and stored it inside their github repo for everyone to use and add into their torrenting software, here are some of the github repo link where they update the torrent tracker:
- [ngosang](https://github.com/ngosang/trackerslist)
- [XIU2](https://github.com/XIU2/TrackersListCollection)

What you gonna do is go to one of the links, for this guide i'll be using [XIU2](https://github.com/XIU2/TrackersListCollection) , after you enter the link you will see this:
![[Pasted image 20250208144525.png]]

Next click 'all.txt' inside this file contains all the trackers:
![[Pasted image 20250208144650.png]]

You can see on the top right inside 'all.txt' before 'history' there is like telling you timing, that mean this file is being update by the owner of the repo so if you see its like months or years that's mean its been updated by months/years ago.

Open your torrenting software, click 'Options':
![[Pasted image 20250208145019.png]]

This window options will show up, and then go to BitTorrent, scroll down till you see 'append these trackers to new downloads':
![[Pasted image 20250208145150.png]]

go back to github repo where you open the 'all.txt', and click the copy button just top right in between 'Raw' and 'Download':
![[Pasted image 20250208145342.png]]

After you copy the file content go back to the Options window of your torrenting software and go to the box just `CTRL` + `V key` in it and click 'apply' and 'ok':
![[Pasted image 20250208145524.png]]

So that's all you need to do, next when you want to download torrent file it will append all that trackers to that torrent file you want to download and your torrenting software will find peers that have torrent file same as you want to download, so you can able to download it.

## Conclusion
This may work and it also depends on the torrent file seeds, as i said on the tips, more seeds faster your downloading is.. good luck :D