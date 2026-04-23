![1](images/software.banner.jpg)

## Operational Relevance

This project demonstrates foundational skills using Windows software tools. Proficiency with Tier-1 and Tier-2 IT Support tasks is demonstrated with screenshots ( click the > dropdowns to view ). Troubleshooting activities are supplemented with ITSM-style tickets which are documented in a companion repository.

(see: [Troubleshooting Journal](https://github.com/robohlstrom24/troubleshooting-journal))

## Tier-1 Job Duties

<details>
  <summary> Troubleshooting High CPU Usage (Task Manager / Performance Monitor / Task Scheduler)</summary>

  **Scenario: A background automation script becomes stuck in a continuous loop while parsing log data, causing high CPU utilization.** 

  ![1](images/highCPU/(1)hook1.png)
  ___________________________________
  ![2](images/highCPU/(2)system-saturated.png)
  _____________________________________________
  ![3](images/highCPU/(3)event-viewer2.png)
  ______________________________________________
  ![4](images/highCPU/task-scheduler.png)
  ____________________________________________
  ![5](images/highCPU/(5)PowerShell-stop.png)
  _____________________________________________
  ![6](images/highCPU/(6)baseline-restored.png)

  **Lessons Leanred:**
  
- High CPU investigations should begin by identifying the top resource-consuming process before taking action
- Performance Monitor helps confirm whether resource spikes are sustained system issues versus temporary application activity
- Investigating automation sources is critical before terminating processes to avoid interrupting legitimate workloads

 See ITSM-style troubleshooting ticket T-0013 in [Troubleshooting Journal](https://github.com/robohlstrom24/troubleshooting-journal)
</details>

<details>
  <summary> Troubleshooting printer failure (Event Viewer / Services) </summary>

The issue:

 ![1](images/logon.failure.png)
 _______________________________

Troubleshooting Steps:

 ![2](images/failure.identified.png)
 _________________________________

 ![3](images/root.cause.png)
 ______________________________

Resolution:

 ![4](images/resolution.png)

 See ITSM-style troubleshooting ticket T-0009 in [Troubleshooting Journal](https://github.com/robohlstrom24/troubleshooting-journal)
 
</details>

## Tier 2 Job Duties

<details>
  <summary>Troubleshooting an Unavailable Web Application (netstat, Services Manager)</summary>

  **Scenario: An internal web application becomes unavailable after the web service hosting the site stops running on the server**

  ![1](images/inaccessible-service/hook(captioned).png)
  ______________________________________________________
  ![2.0](images/inaccessible-service/insert-2.png)
  _____________________________________________________
  ![2](images/inaccessible-service/(1)none-listening.png)
  _____________________________________________________
  ![3](images/inaccessible-service/(2)service-not-running.png)
  ___________________________________________________
  ![4](images/inaccessible-service/(3)service-restarted.png)
  ___________________________________________________________
  ![5](images/inaccessible-service/(4)port-listening.png)

**Lessons Learned:**
- Verifying whether a service port is listening is a quick way to determine if an application is accepting connections
- Network tools like netstat can help distinguish between connectivity issues and application/service failures
- Understanding which services support critical applications helps speed up root cause identification

   See ITSM-style troubleshooting ticket T-0014 in [Troubleshooting Journal](https://github.com/robohlstrom24/troubleshooting-journal)
</details>
