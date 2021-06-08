a---
title: Assignment 1
subtitle: Computer performance, reliability, and scalability calculation
author: Brett Sutow 
---

## 1.2 

#### a. Data Sizes

| Data Item                                  | Size per Item | 
|--------------------------------------------|--------------:|
| 128 character message.                     | 128 Bytes one character equals 1 byte|
| 1024x768 PNG image                         | 1.573 MB equals 1024x768=   786432 *2 thenconvert to MB from bytes to get 1.573  |
| 1024x768 RAW image                         | 1.5 MB equals (1024 * 768 * 16 )  / ( 8   * 1024) ) / 1024      | 
| HD (1080p) HEVC Video (15 minutes)         |  89,568MB 167,940/1.5(compression rate)= 89,568 MB I utilized the folllowing online video to file convertor: https://toolstud.io/video/    for all the video formulas     |
| HD (1080p) Uncompressed Video (15 minutes) |  167,940 MB = 6.22MB * 27,000frames = 167,940MB        |
| 4K UHD HEVC Video (15 minutes)             | 1,519 MB   0.05625 * 27,000= 1,519 |
| 4k UHD Uncompressed Video (15 minutes)     |2,278.125 MB   I utilized the folllowing online video to file convertor: https://toolstud.io/video/    for all the video formulas 1,519 * 1.5 (compression rate)      |
| Human Genome (Uncompressed)                | 200 GB   This was found on the following site where they simplified forumula taking 90GB of space for the human geonme: https://medium.com/precision-medicine/how-big-is-the-human-genome-e90caa3409b0        |

#### b. Scaling

|                                           | Size     | # HD | 
|-------------------------------------------|---------:|-----:|
| Daily Twitter Tweets (Uncompressed)       | 640,000 MB   192 HDs 128 * 500mill = 6,400,000,000 bytes * 3 HDs = 192,000,000/1mill   |      |128 * 500mill = 6,400,000,000 bytes * 3 HDs = 192,000,000/1mill
| Daily Twitter Tweets (Snappy Compressed)  | 426,666 MB | .128 HDs  6,400,000,000/1000/1.5=426,666 * 3 HDs= 1,280,000   | 6,400,000,000/1000/1.5=426,666 * 3 HDs= 1,280,000
| Daily Instagram Photos                    | 820,425MB  | .820 HDs 75k *  1.573mb + 25k * 6.22 = 117,975 + 155,500/1mill    | 75k *  1.573mb + 25k * 6.22 = 117,975 + 155,500/1mill
| Daily YouTube Videos                      | 4,299,264,000MB|  4299.264HDs   500Hrs * 60min = 30,000 min/15min video= 2,000 videos x 89,568MB*24hrs   | 500Hrs * 60min = 30,000 min/15min video= 2,000 videos x 89,568MB*24hrs 
| Yearly Twitter Tweets (Uncompressed)      | 233,600,000MB|70,080 HDs      |
| Yearly Twitter Tweets (Snappy Compressed) | 155,733,090MB| 46.72 HDs     |
| Yearly Instagram Photos                   | 299,455,125MB       |     299.3 HDs |
| Yearly YouTube Videos                     | 1.5692314e+12MB       | 1,569,231.36HDs|

#### c. Reliability
|                                    | # HD | # Failures |
|------------------------------------|-----:|-----------:|
| Twitter Tweets (Uncompressed)      | 70,080   |    595.68        |
| Twitter Tweets (Snappy Compressed) | 46.72   |     .39712       |
| Instagram Photos                   | 299.3   |     2.54405       |
| YouTube Videos                     | 1,569,231   |    13,338.46        |

#### d. Latency

|                           | One Way Latency      |
|---------------------------|---------------------:|
| Los Angeles to Amsterdam  | 139.545ms                |https://wondernetwork.com/pings/Los%20Angeles/Amsterdam
| Low Earth Orbit Satellite | 600 ms                 |https://www.omniaccess.com/leo/
| Geostationary Satellite   | 250 ms               |https://web.archive.org/web/20160103125227/https://www.isoc.org/inet97/proceedings/F5/F5_1.HTM
| Earth to the Moon         | 2520 ms  |https://www.forbes.com/sites/quora/2016/08/31/when-we-eventually-get-to-mars-this-is-how-the-internet-will-work-there/?sh=aee08617dae7
| Earth to Mars             | 20 minutes            | https://mars.nasa.gov/mer/mission/timeline/surfaceops/navigation/


References: https://wondernetwork.com/pings/Los%20Angeles/Amsterdam
https://medium.com/precision-medicine/how-big-is-the-human-genome-e90caa3409b0    
https://web.archive.org/web/20160103125227/https://www.isoc.org/inet97/proceedings/F5/F5_1.HTM
https://mars.nasa.gov/mer/mission/timeline/surfaceops/navigation/
https://www.omniaccess.com/leo/
https://www.forbes.com/sites/quora/2016/08/31/when-we-eventually-get-to-mars-this-is-how-the-internet-will-work-there/?sh=aee08617dae7

https://toolstud.io/video/
