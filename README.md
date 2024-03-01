<h1> GUIDE - FOSS LED controller </h1>
A guide on how to build a controller for you LEDs and control it using Wled. 

<!-- description -->
<div>
  <p>
    Huge shout-out to <a target="_blank" href="https://github.com/Aircoookie/WLED">Aircoookie</a> and his <a target="_blank" href="https://github.com/Aircoookie/WLED">WLED repository</a>. You should definetely go check his repository. 
  </p>
  <p>
    This guide summarizes how I build a controller for my LED strip and gives you step by step DIY instructions how to do the same.
  </p>
  <p>
    If you are more of a visual person you can also check the guide on <a target="_blank" href="https://www.youtube.com/watch?v=_wZEJPShvmI">Makers Mashup</a> channel.
  </p>
</div>

<!-- Index-->

Index
<h4>
  Table of Contents
</h4>
  - [What you need](#what-you-need)



<!-- List of components needed -->
<h4>What you need</h4>
<ul>
  <li>
    <a target="_blank" href="https://www.amazon.de/dp/B0CH9JYNMH?psc=1&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=5e8e8686c2825231051a55fb24c847f2&camp=1638&creative=6742">ESP32</a><a target="_blank" href="https://www.amazon.de/dp/B01CDTEFAQ?psc=1&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=b3f8b093f5ddb8f3de39363ae62fabd5&camp=1638&creative=6742">BTF lighting LED strip</a>
  </li>
  <li>
    <a target="_blank" href="https://www.amazon.de/-/en/Gebildet-Electric-Flexible-Connection-Oxygen-Free/dp/B0BG3W15YT?dib=eyJ2IjoiMSJ9.1KIqM_msf5bOJzSkH1ew8mpkRV9ON6T-JkpoG9VBrVNiQsBOy89PVl9_OxJ3WE52dZQ2NwPvhQfohTIVtA9uTdrEeeiJJAPTrq25blI_kGLVwsQcBmtw9uFV5yNYrgs_dZ3xnOrRc1s9acYoimm7y3bca-84lVwHo9U46wYOgbKhuAMUjt-Xy6J_0iJHgT5fWcUpq3opJyRQpXT_dCYemLRv1_L1Vhb6aBbEgtndBn2SdkT2JgZK1j0tg-6RY1d7_cKGvbd6RSDbv6b0286VtzrH7L6tx3arj0Nl6txS4KA.qZ71FKLbXAXQjmTYETNYcB8YM56PsqjJkf6iahdto4Q&amp;dib_tag=se&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=576c6aababe3138b3a46847e62dd7fc6&camp=1638&creative=6742">22AWG cable</a>
  </li>
  <li>
    <a target="_blank" href="https://www.amazon.de/-/en/ELECTROCOOKIE-Solderable-Chopping-Electronics-Gold-Plated/dp/B07ZV8FWM4?dib=eyJ2IjoiMSJ9.R8hifUH4Z4qV9mqzrm8pVhDFbzQceLYM5MTMFrhtIJ_TUnCFGWB4L2hBIKa5Kvxg9CJFdvNoug8qikf_ctEGvEToVgCKg-ne8Q_VB1-ZWeL6DX10raUdNJ_N66KOxJEF3Fnw6C_Cle0v2xN8uNRN08peYrERas7X0KwwmtmGJ8bSHUUgeLFxoYTy6OaHKGxBDL8XnqQ_XeBmko_0kLd10P6hJlL349v9eJYQZcgpcrqBEKb8CvrxGSpQe73oA-2bh7iFQ0sCTnmDmMb1hwucuTw0B6XMj__RIquTRz2JRgQ.OutE2IY-4E1z_wexHk4j18ZhPaH_eyhJy9p5aLWQquk&amp;dib_tag=se&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=06c6f7d91402c0890aab6fb216574041&camp=1638&creative=6742">Solderable Bread Chopping Board </a>
  </li>
  <li>
    <a target="_blank" href="https://www.amazon.de/dp/B00LPWIM98?psc=1&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=211c7eebfa54a5625c0967cfe80e132f&camp=1638&creative=6742">1000 uF Capacitor</a>
  </li>
 <li>
   <a target="_blank" href="https://www.amazon.de/-/en/3PIN-SM/dp/B01DC0KIT2?dib=eyJ2IjoiMSJ9.UtMqHJDKSZoZ1n7XYeASs_LOCJQviBdJ2hbNelUnE73aG3rCD2k4SYQxh5w89FOuyeTolSPvgeRr88dwWai2-tWnz33-2M6h_oGuuPVpzzXFwXpagqb7qjM5qO7-u7ZKpqTWJ-0T5FA_4RVL1t9M8rTS5mZ1R7pzq-v4Z1PVxczj0gB07y3TvFEXha4Ma6Hn-vvfgxE_WxRjtzSHInapuLMN1ENZxhq4laLXCe-2Baaus1DBMZZRVC7TQeVT7PgHQrogDc2XGGtKN52d0spcW8_FYQVx8QX0DByOLJLaXmg.Fhwc6EovLJEJ3IFUYlHUDwpyZz8oSAg3lMohqoosjO0&amp;dib_tag=se&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=765d2f649aec2928511a67563f6c5e24&camp=1638&creative=6742">3 pin LED connector</a>
 </li>
  <li>
    <a target="_blank" href="https://www.amazon.de/dp/B09CH8QBJN?&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=ec213bb0bc51d7d075939477411e1021&camp=1638&creative=6742">Case</a>
  </li>
  <li>
    <a target="_blank" href="https://www.amazon.de/-/en/17893/dp/B003H9CJ1Y?dib=eyJ2IjoiMSJ9.1R0jS4Qs2cda5Vry4e1XR3COvrSttgudBiP6oy1Mad84Zw80DkovYrZlh-LTGmDObYHKzmLY02CbwRUElC7DvjP1ZpMLxtXfm66u__qt7EJGdxD6i2rd_7U7iJV1iZhzpi6uxOvsppBPs6iT4oZ1NE06-uFc0DGiXmy0irFDYA5T7iMKS1q2xbN8xgjwafnaACx-EreX4KyT36zUPXP1ZQM2I6HtFLZ_LuG0e4sMeG3TNhbvlM_uIBCj0a8z3YPgdLNLqRnWwaiH2hI7sIJ_uMrzeEJ7utU9OKtCIQHUXCU.uLzurU4WGO1fWf42sTHAUK-8oSEZfgObOKKGq2DNjWU&amp;dib_tag=se&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=4cc363e9362d0626f88950d4f2d42cf8&camp=1638&creative=6742">Heat shrink tube</a>
  </li>
  <li>
    <a target="_blank" href="https://www.amazon.de/-/en/Assortment-Stackable-Breakaway-Arduino-Prototype/dp/B07CWSXY7P?dib=eyJ2IjoiMSJ9.9S4dcSq_QjxNncwZaJt6LTsVEFLR6baM750-POiAPlTPRPMnXLWtuxgnXBOPSBLyXXEgesAwi7zr4cv_vRUaGKAKq7RMpNaNNVFt6BvwNjD2UkL85pTaZbAqTLigxbXSAOpCCBjd_lSMX6Xvc5r1dG153KQfdZ9hlhbF3WYC-RdcKYDwn8ThsslTZH-A36A951nUj0_Od-f4iKntVeMwEADftXnAPBg32junYtkZsnJr-Xo4437rW_1z7pjYSsKHBvpfrsm0i6l6O8bt0r23vpB-6aJrWDnbdVLw4m9gleA.S8EH7mYp2sJtMj58zSWPIOzfWFB6FEunUeBjXi6NWEw&amp;dib_tag=se&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=63876dabbd4d9554c9ce62958c4daa03&camp=1638&creative=6742">Pin Header </a>
  </li>
  <li>
    <a target="_blank" href="https://www.amazon.de/-/en/Female-Socket-Adapter-Camera-Connector/dp/B0BR6PQ64L?dib=eyJ2IjoiMSJ9.xtkUgB1ky1P8tc5s6qeKrgIpzcyIA9Xhy6qzCY3h6sHoPLDgMCGV3CA5KY31nTPmz9NJ5LrlSj08RFL5E6lOE6DL1W9_FWHJoY2gtFOa6mcqHuA37a0TqhXYcXqrXqxqlW1sEJH-5FwJEJlg3UF_xr0qTZM8Z2-D39HB_8Dtyg8yCVU9gcd7iftaoUhs4yjgJoS3sK-xJ2BGEnGRewl7TAtu5OFMQnfKjtuMatmZwwM.88Hvhw5fT4OJ7XrCiFp1HHDeUyVXpAIQQyvYxa94d5g&amp;dib_tag=se&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=7c92873d73a4de67695ca3c6d5a25988&camp=1638&creative=6742">Female DC plug connector</a>
  </li>
  <li>
    <a target="_blank" href="https://www.amazon.de/-/en/Switching-100V-240V-Universal-Transformer-Cordless-5-V-2-pieces/dp/B0BK9Q7S7C?dib=eyJ2IjoiMSJ9.MuJPF2nk797D8SB68dCuU6pESXZkdWflvJ5wWsCqpfgP0XaXGdqGNUW_5HB2ltISqnOiuvACVHedkRojFlRPdcPPd88zdwPJ0puYbjitP_RhLDPK74johAlDyieK5EjOG1lS8Hx-b-Um5zwvJOtWURMhBlQkAdwChCBOVeJe6TwDOg9le1zn3yaW9yIw8m0jQ9FbVk8sLRanvkzSvbBXsaWYtlJJCzsaTZWm1K-JTFYBpIGQfZfySsI6xeo6ls2ipfGwikGW4V14DZ8TxPAkC5RVVgC3PVuBBZQpt14zcl8.QEH9vBQViOvQ2_pwbXfh69gI2b73HjpJXNfiifj2cgA&amp;dib_tag=se&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=43ddafd6e9e31534e84c4d84b92d70bf&camp=1638&creative=6742">5V (2A) Power supply adapter </a>
  </li>
  <li>
    <a target="_blank" href="https://www.amazon.de/gp/product/B09CKTYTVJ?psc=1&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=af94a1985c185519fb49b90e8135d98a&camp=1638&creative=6742">Soldering Iron (a basic kit like this would do the job)</a>
  </li>
  <li> 
    <a target="_blank" href="https://www.amazon.de/-/en/KX1650-QS/dp/B004XZFZL2?dib=eyJ2IjoiMSJ9.6_3pvUAPvgLmuM6bTS-6orW4c7AqlDlIyZhdIQgcOcPUk73jSQQarBxr5BaFTKnVKc5WOQduULp3i0eJ5Nn53ay3H7uionF4Iz2eFeWDApCzjk--W60XNghmwJGmTrq3HDhCKBI2ILhez5A60M7XLVeXwDXxvTmCwpEjYi9Vo4wZT3ZQKVVSaWEfLaknDpVbWQCzXu1iKt0wYttrTip3MyUzbdlCq3c1CRI9pibUjEI.W23293o5taMBLDBOsPx_EJ_auIy54M_Rsp74nNF3msk&amp;dib_tag=se&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=26f122594f93b4ca88e5c517d80f5f2b&camp=1638&creative=6742">Heat gun (an hair dryer also works)</a>  
  </li>
  <li> 
    <a target="_blank" href="https://www.amazon.de/gp/product/B000EBN174?psc=1&_encoding=UTF8&tag=flhub-21&linkCode=ur2&linkId=343df24964547b315cc2deefd445b94e&camp=1638&creative=6742">Drill</a>
  </li>
</ul>

<h6>
  Disclaimer: Some of the links above are affiliate links. This means that, at zero cost to you, I will earn an affiliate commission if you click through the link and finalize a purchase.
</h6>




