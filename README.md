<p align="center">

![image](https://github.com/Loughton03/soc-active-directory/assets/78968473/64f88fee-1609-404f-af0f-0506064577d4)

</p>

<h1>Microsoft Entra ID (Azure Active Directory) Overview (Users, Groups, and Access Management)</h1>
In this part, we will explore Azure Active Directory (AAD) and observe different access levels..<br />

<h2>What is Microsoft Entra ID (Azure Active Directory)?</h2>

-  Microsoft Entra ID is a cloud based identity and access management service.

<h2>Actions and Observations</h2>

<h3>Azure Logging at Different Layers: We will set up logging at the Tenant global reader level, Activity, and Resource levels to capture essential events and activities.</h3>

<p>
1. We will start with setting up logging at the tenant global reader level:
 - create a new user named Logan
</p>

<p>
<img src="https://i.imgur.com/4z5cbQr.png" height="80%" width="80%" alt="Resource Group Setup"/>
</p>

<p>
<img src="https://i.imgur.com/4izYlf3.png" height="80%" width="80%" alt="Resource Group Setup"/>
</p>


<p>
<img src="https://i.imgur.com/M7fAk1R.png" height="80%" width="80%" alt="Resource Group Setup"/>
</p>

<p>
2. Assign the role of global reader to our new tenant
</p>
<br />

<p>
<img src="https://i.imgur.com/IJthm4I.png" height="80%" width="80%" alt="Virtual Machine Setup"/>
</p>

<p>
<img src="https://i.imgur.com/yLGds5H.png" height="80%" width="80%" alt="Virtual Machine Setup"/>
</p>

<p>
<img src="https://i.imgur.com/tJDJoGM.png" height="80%" width="80%" alt="Virtual Machine Setup"/>
</p>


<p>
3. we will observe the results of being a gloabl level tenant by accessing azure from a incognito browser function. We will need the user principal name, which is the user name, to access the portal.azure.com
</p>
<br />

<p>
<img src="https://i.imgur.com/mwvp2mi.png" height="80%" width="80%" alt="Virtual Machine Setup"/>
</p>

<p>
<img src="https://i.imgur.com/TWqUyNC.png" height="80%" width="80%" alt="Virtual Machine Setup"/>
</p>

<p>
 *After logging in you will be prompted to create a new password. You willl notice your rights are restricted as a global level tenant. For example you do not have the ability to view azure subscriptons. When done viewing you can close the incognito window.
</p>

<p>
4. Create another user within Microsoft Entra ID and assign them subscription-level reader
 <ul>
 <li>Assign them username: subreaderkim</li>
 <li>Auto generate a password, you will be prompted to create a new password when logging in</li>
 <li>Review and create the user</li>
 </ul>
</p>

<p>
<img src="https://i.imgur.com/1lVk2wu.png" height="80%" width="80%" alt="Virtual Machine Setup"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/z5gNW94.png" height="80%" width="80%" alt="Virtual Machine Setup"/>
</p>
<br />

<p>
<img src="https://i.imgur.com/AtHNmOE.png" height="80%" width="80%" alt="Virtual Machine Setup"/>
</p>
<br />

<p>
5. We will Assign the subscription level reader role to our user kim through our subscrption list
</p>

<ul>
 <li>Move to the subscriptions tab</li>
 <li>Click on Access controls(IAM)</li>
 <li>Then add role assignment</li>
 <li>In a incognito browsesr, log into subreader kim and observe results of being a Subscription Level Global Reader</li>
</ul>

<p>
<img src="https://i.imgur.com/vRqv4EB.png" height="80%" width="80%" alt="Virtual Machine Setup"/>
</p>

<p>
<img src="https://i.imgur.com/HtdKZaX.png" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
<img src="https://i.imgur.com/l5waZbn.png" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
<img src="https://i.imgur.com/gQOdlOL.png" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
<img src="https://i.imgur.com/ly1gZQU.png" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
<img src="https://i.imgur.com/5cUDH50.png" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
6. We will create a new user, Michael, and assign him Resource group level contributor permisssions.
</p>

 <ul>
 <li>Assign him username: rgcontributormichael</li>
 <li>Auto generate a password, you will be prompted to create a new password when logging in</li>
 <li>Review and create the user</li>
 <li>Create a new resource group called "Permissions-Tester</li>
 <li>Assign permissions through the newly creatd resource group</li>
 <li>In a incognito browsesr, log into Michael and observe results of being a Resourse Level Contributor</li>

 </ul>
 
<p>
<img src="https://i.imgur.com/O0FYVbY.png" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
<img src="https://i.imgur.com/hrLShl6.png" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
<img src="https://i.imgur.com/iHq6pmM.png" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
<img src="https://i.imgur.com/00tToxi.png" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
<img src="https://i.imgur.com/tpRqT0c.png" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
<img src="https://i.imgur.com/nfLYizS.png" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
<img src="https://i.imgur.com/aGCsshl.png" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
<img src="" height="80%" width="80%" alt="Public IP Address"/>
</p>

<p>
7. Subscription Level Logging: We will configure logging at the subscription level to gain insights into events and activities specific to each subscription.
</p>

<p>
<img src="https://i.imgur.com/epjhJof.png" height="80%" width="80%" alt="Public IP Address"/>
</p>







