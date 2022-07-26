# qa-best-practices
Ths repository will consist of a QA documentation, example templates and best qa practices.

Sources:
https://www.freecodecamp.org/news/how-to-write-qa-documentation-that-will-work/

Начини на репортване на бъговете:
Намерените бъгове се качват в Jira, QA Board под формата на defect report. Всеки отделен фийдбек съдържа следните компоненти:
* имейл на потребителя/тестовия акаунт;
* URL на страницата където е намерен проблема;
* устройството на който е намерен дадения бъг /десктоп или мобилна версия/;
* стъпки за пресъздаване на проблема;
* скрийншот на проблема;
* допълнителна информация около пресъздаване/fix-ване на проблема;

NB! Ако дадения бъг е намерен на production, то той:
* в момента на писане на документацията той се описва по-горе посочените начини и се качва в QA канала с цел по-бързото му fix-ване.
* при репортнат проблем от потребител в helpscout, то проблема се качва под формата на тикет в GitHub, като му се прилагат нужните тагове ("helpscout", "enhancement", и т.н.)

т1: Комуникация, видове:

* при fix-нати неща от QA фийдбек-a;
* при deploy на staging или production;
* при deploy на Hot Fix на production;
* при невъзможност/въпросителни относно даден бъг в QA фийдбека;
* обсъдена важна промяна с клиента, която не е описана в Jira ticket, GitHub тикет и др.

т3: Начин на тестване:

QA отваря тикета с комуникация (GitHub, Jira и т.н.) и започва последователно да преглежда точките по които ще се работи в дадения бъг/feature;
т4: Тестване след Deploy на Production:
т1: Комуникация, видове:
- при fix-нати неща от QA фийдбек-a;
- при deploy на staging или production;
- при deploy на Hot Fix на production;
- при невъзможност/въпросителни относно даден бъг в QA фийдбека;
- обсъдена важна промяна с клиента, която не е описана в Jira ticket, GitHub тикет и др.

т3: Начин на тестване:

- QA отваря тикета с комуникация (GitHub, Jira и т.н.) и започва последователно да преглежда точките по които ще се работи в дадения бъг/feature;

т4: Тестване след Deploy на Production:

QA Documentation steps:
The documentation saves a ton of time by streamlining your testing processes. It’s, also, your go-to asset in case something goes off the rails with the project.

Now, let’s continue our deep dive into writing a QA documentation. Five more topics:

* Defect Reports
* The Life-cycle of a Defect Report
* Typical Errors When Creating a Defect Report
* Test Plans
* Test Progress Report

1. DEFECT REPORTS
A defect report is a road-map for getting bug-free software. In short, the report describes any unwanted issue with your solution. It sounds simple until you start documenting. Below you can see an example of a typical defect report.

Let’s go through every section of the defect report:
The identifier is your unique value for recognizing a specific defect report in a sea of others.
The summary is your laconic answer to three simple questions “What happened?”, “Where?” and “Under what circumstances?”.
The description is where you show the bug in all the details. You should describe the actual and expected results. Moreover, it’s a good idea to provide a link to your software requirements.
Then, you write about the steps to reproduce (STR). Don’t miss a step or your report may end up in a trash folder. ??
In the reproducibility, you show if the bug appears every time you follow the STR.
The severity shows how harmful the bug is to the project. Don’t exaggerate because if the developer notices, your report might end up the last in the queue.
The priority shows the urgency, and it’s a logical addition to the severity section.
The symptom is a short label to stack your defect report with the other similar reports.
Also, you should be a good tester and describe workarounds if you know about any.
The comments can include all the useful information for your developer.
Finally, the attachments include the list of files added to the defect report.
At the end of the day, you will come up with a report like one below. This report is from Jira, one of the many wonderful project management tools.


2. THE LIFE-CYCLE OF A DEFECT REPORT
Submitting is only the first step before fixing the bug once and for all. There’s a whole life-cycle.

You start by submitting your defect report. Next, your project team has the option of either assigning it to a developer or declining the report. If your defect report is not a total mess, your team will accept it. Then, the assigned developer can either start fixing the bug or try to decline your report again. Usually, it’s your tech lead who decides if there are enough reasons for declining. Moreover, the tech lead has the power to defer any defect report under the pretense it’s not relevant.

Congrats! You’ve forced the developer to fix the bug. What next? You have to double-check the bug fix and verify if all is good. If not, you have to start all over again and reopen the defect report. This bug-fixing battle can be a long one. You can, finally, close the defect report only after about a week or two after a proper bug fix.

This defect report life-cycle is definitely not set in stone, and it should reflect the needs of your project. Be smart!


3. TYPICAL ERRORS WHEN CREATING A DEFECT REPORT
There are dozens of mistakes testers make in a defect report. Yet, only a couple of them are typical and persisting. Let’s go through the typical errors when creating a defect report:

A short and inadequate summary.
The summary and the description are pretty much the same.
The description has no expected result, no actual result, and no link to requirements. Nothing at all.
A print screen has no issue highlighted. This way, the developers might as well play ‘Find Waldo’ with the issue.
Describing imaginary defects.
Putting away your work for tomorrow, and the day after tomorrow, and …. you get the idea.
Making grammar mistakes. This is the easiest way to get shot by a grammar nazi.
Describing features as bugs because you know it’s the best way to get fired.
Not knowing the technical requirements of the tested solution. This type of tester is no better than this little dog-o below.
Missing out important information in your Steps to Reproduce.


4. TEST PLANS
Now you know all about defect reports and, hopefully, about test cases and test suits too. It’s time to give you the big picture of QA documentation. It’s time to make a test plan.

Your test plan should be your guiding document. It should include your to-do-list, strategy, resources, schedule and much more.

Your average test plan should answer thirteen questions:
What is the purpose of the software solution? Is there any?
What features should you test? Don’t go on a testing frenzy and test everything.
How does the testing process look like? What are the methodologies, approaches, technologies, tools and so on?
What are the acceptance criteria of your customer or your target audience?
When should you start and finish testing?
What are the criteria for stopping and continuing tests? Do you stop testing when you’re out of cookies?
What development resources do you need? What OS, how many copies and with what license? Yes, you have to worry about all of this.
What hardware and what experts do you need? Look for the best in class.
How much time and money does your project have for testing? Is it worthwhile?
Is there a test schedule? Perhaps, you should consider cramming all your testing into one day before deployment.
Are your roles and responsibilities well designated? Who’ll do the job, if your lead tester disappears?
Are there any testing risks? Is it risk-free not to test at all? 
What are the metrics and QA documentation your using? Maybe, go Rambo and document nothing.


5. TEST PROGRESS REPORT

The test progress report is like a test plan but with the current progress data added for comparison. In short, the report is a great way to keep your hand on the pulse of a project. So, you must mention eight things in your test summary report and you’re off to success.
