
  @verbatim
  ******************************************************************************
  *  
  *           Portions COPYRIGHT 2016 STMicroelectronics                       
  *           Copyright (c) 2001-2004 Swedish Institute of Computer Science, All rights reserved.
  *                                                                      
  * @file    st_readme.txt 
  * @author  MCD Application Team
  * @brief   This file lists the main modification done by STMicroelectronics on
  *          LwIP for integration with STM32Cube solution.
  *          For more details on LwIP implementation on STM32Cube, please refer 
  *          to UM1713 "Developing applications on STM32Cube with LwIP TCP/IP stack"  
  ******************************************************************************
  *
  * Redistribution and use in source and binary forms, with or without 
  * modification, are permitted, provided that the following conditions are met:
  *
  * 1. Redistribution of source code must retain the above copyright notice, 
  *    this list of conditions and the following disclaimer.
  * 2. Redistributions in binary form must reproduce the above copyright notice,
  *    this list of conditions and the following disclaimer in the documentation
  *    and/or other materials provided with the distribution.
  * 3. Neither the name of STMicroelectronics nor the names of other 
  *    contributors to this software may be used to endorse or promote products 
  *    derived from this software without specific written permission.
  * 4. This software, including modifications and/or derivative works of this 
  *    software, must execute solely and exclusively on microcontroller or
  *    microprocessor devices manufactured by or for STMicroelectronics.
  * 5. Redistribution and use of this software other than as permitted under 
  *    this license is void and will automatically terminate your rights under 
  *    this license. 
  *
  * THIS SOFTWARE IS PROVIDED BY STMICROELECTRONICS AND CONTRIBUTORS "AS IS" 
  * AND ANY EXPRESS, IMPLIED OR STATUTORY WARRANTIES, INCLUDING, BUT NOT 
  * LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY, FITNESS FOR A 
  * PARTICULAR PURPOSE AND NON-INFRINGEMENT OF THIRD PARTY INTELLECTUAL PROPERTY
  * RIGHTS ARE DISCLAIMED TO THE FULLEST EXTENT PERMITTED BY LAW. IN NO EVENT 
  * SHALL STMICROELECTRONICS OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT,
  * INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT
  * LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, 
  * OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF 
  * LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING 
  * NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE,
  * EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
  *
  ******************************************************************************
  @endverbatim

### 22-April-2016 ###
=====================
  + Use updated version of LwIP v1.4.1 by integrating latest sources from LwIP Git Repository: 
    - Integrate latest commit dated of 2016-02-11, reference http://git.savannah.gnu.org/cgit/lwip.git/commit/?id=cddd3b552a52027a503a00982ceaaec9a6959819
    - Main new features:
      - IPv6 support.
      - Dual IPv4/IPv6 stack.
      - Optional use of IPv4. 
    - Many Bugs fixing an enhnacement, for more detailed please refer to CHANGELOG file
    - Updated architecture having impact on application based on previous version:
      - dhcp.c file is now available under \src\core\ipv4 directory
      - inet_chcksum.c is now available under \src\core directory
      - ip.c and ip_addr.c are renamed to ip4.c and ip4_addr.c respectively.
      - SNMP, SNTP and HTTP protocols implementation is available under \src\include\lwip\apps directory
 
### 19-June-2014 ###
====================
  + sys_arch.c file: fix implementation of sys_mutex_lock() function, by passing "mutex"
   instead of "*mutex" to sys_arch_sem_wait() function.  


### 18-February-2014 ###
========================
   + First customized version for STM32Cube solution.


 * <h3><center>&copy; COPYRIGHT STMicroelectronics</center></h3>
 */
