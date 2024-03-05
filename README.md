<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1 align="center">osTicket - Understanding Ticket Lifecycle</h1>
This guide illustrates the stages of a ticket's lifecycle, from initial intake to resolution, within the osTicket help desk ticketing system. It is assumed that you have already completed both the <a href="https://github.com/jadeblas/osticket-prereqs">installation</a> and <a href="https://github.com/jadeblas/post-install-config">configuration</a> of osTicket.

</br>

<h2>Environments and Technologies Used</h2>
<ul>
  <li>Microsoft Azure (Virtual Machines/Compute)</li>
  <li>Remote Desktop</li>
  <li>Internet Information Services (IIS)</li>
  <li>osTicket</li>
</ul>

</br>

<h2>Operating Systems Used</h2>
<ul>
  <li>Windows 10</li>
</ul>

</br>

<h2>Ticket Lifecycle Stages</h2>
<ol>
  <li>Intake</li>
  <li>Assignment & Communication</li>
  <li>Working the Issue</li>
  <li>Resolution</li>
</ol>

</br>

<h2>Detailing Lifecycle Stages</h2>

<h3>Intake</h3>

<p>
  <ul>
    <li>End users, such as Karen Karen, initiate ticket creation via osTicket's local host site. They provide their information and select a suitable Help Topic.</li>
    <ul>
      <li><img src="https://github.com/jadeblas/ticket-lifecycle/assets/161860082/e98de2de-8a4d-4853-b094-cfb531489019" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>The end user then fills in the ticket's details, including an Issue Summary with subject and details similar to composing an email.</li>
    <ul>
      <li>In this scenario, Karen submits a ticket under the Help Topic "Business Critical Outage" (configured in osTicket), reporting a 404 error in the mobile banking application.</li>
      <li><img src="https://github.com/jadeblas/ticket-lifecycle/assets/161860082/6466c1dc-180a-4823-9e81-4c901165775e" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>The ticket is then assigned to Agent Jane Doe (configured as a Supreme Admin with access to all incoming tickets) who views it via the local help desk login.</li>
    <ul>
      <li><b>Note</b>: Priorities have not been assigned for other incoming tickets, such as ticket #951342 where end user Ken is requesting an upgrade to Adobe Reader. SLA plans need to be configured for these tickets, hence they are all categorized under the "Normal" priority state.</li>
      <li><img src="https://github.com/jadeblas/ticket-lifecycle/assets/161860082/f5fb2102-55c9-4a6c-9e85-c150ce0487e0" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
  </ul>
</p>

<h3>Assignment & Communication</h3>

<p>
  <ul>
    <li>The ticket #282733, a Business Critical Outage reported by Karen, is assigned to Agent Jane Doe. Here's how the ticket appears from Jane's perspective:</li>
    <ul>
      <li>Jane can communicate with the end user through the <b>Ticket Thread</b> located at the bottom of the ticket page.</li>
      <li><img src="https://github.com/jadeblas/ticket-lifecycle/assets/161860082/63bb6183-855c-4f13-b55a-e15356981c13" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>She can adjust the ticket's priority by clicking on the link next to <b>Priority</b>, choosing from Low, Normal, High, or Emergency.</li>
    <ul>
      <li><img src="https://github.com/jadeblas/ticket-lifecycle/assets/161860082/4c3aadfa-a3df-443c-adea-bc42973c4cf2" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>Assigning the ticket to a team or agents is possible by clicking on the greyed-out link --Unassigned-- next to <b>Assigned to</b>. Note that if the ticket is assigned to an agent outside of Jane's department, it won't appear in their feed.</li>
    <ul>
      <li><img src="https://github.com/jadeblas/ticket-lifecycle/assets/161860082/b23c8057-2b5b-421f-a298-c62c335aa129" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>Jane can also set the SLA Plan by clicking on the link next to <b>SLA Plan</b> and choosing one of the SLA Plans created during configuration. For this Business Critical Outage ticket, it'll be set to SEV-A.</li>
    <ul>
      <li><img src="https://github.com/jadeblas/ticket-lifecycle/assets/161860082/253bceb1-b531-435b-ad7f-806706ce8968" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>Setting the department is done by clicking on the link next to <b>Department</b>. For this Business Critical Outage ticket, it'll be changed from Support to System Administrators.</li>
    <ul>
      <li><img src="https://github.com/jadeblas/ticket-lifecycle/assets/161860082/294efa2b-ca93-4e25-93f8-1dda2f1f57a5" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>The Ticket Thread is updated each time a change is made to the ticket.</li>
    <ul>
      <li><img src="https://github.com/jadeblas/ticket-lifecycle/assets/161860082/d173847c-e0a8-4fec-aff1-e6da8730fa6e" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>Jane can communicate with the end user through the Ticket Thread to provide updates on the ticket status. The status remains <b>Open</b> as it requires further attention.</li>
    <ul>
      <li><img src="https://github.com/jadeblas/ticket-lifecycle/assets/161860082/146ae2fd-2b79-4963-a14d-81351d3a441f" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
  </ul>
</p>

<br />

<h3>Resolution and Closing</h3>

<p>
  <ul>
    <li>After handling the issue and communicating with the end user, the critical banking outage ticket is resolved with the assistance of the System Engineering team. The agent must update the end user about the resolution through the Ticket Thread and change the ticket status from Open to <b>Resolved</b>. Once the reply is posted, the ticket is marked as <b>Closed</b>.</li>
    <ul>
      <li><img src="https://github.com/jadeblas/ticket-lifecycle/assets/161860082/4f1defc4-71ea-4836-ae4b-414e31951017" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
    <li>Closed tickets are archived in the Closed section of the Tickets tab, containing all pertinent information and status updates. Agents are encouraged to review closed tickets to enhance their handling skills.</li>
    <ul>
      <li><img src="https://github.com/jadeblas/ticket-lifecycle/assets/161860082/21276138-5dbe-4999-8191-c5c3a8b6a8aa" height="80%" width="80%" alt="Disk Sanitization Steps"/></li>
    </ul>
  </ul>
</p>

<br />
