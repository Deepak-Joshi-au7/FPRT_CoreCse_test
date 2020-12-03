Ques 1:- What is OWASP? And explain the top to Owasp.

Answer:- The Open Web Application Security Project, or OWASP, is an international non-profit organization dedicated to web application security. One of OWASP’s core principles is that all of their materials be freely available and easily accessible on their website, making it possible for anyone to improve their own web application security. The materials they offer include documentation, tools, videos, and forums. Perhaps their best-known project is the OWASP Top 10.

top 2 Owasp are:

1. Injection:
   Injection attacks happen when untrusted data is sent to a code interpreter through a form input or some other data submission to a web application. For example, an attacker could enter SQL database code into a form that expects a plaintext username. If that form input is not properly secured, this would result in that SQL code being executed.Injection attacks can be prevented by validating and/or sanitizing user-submitted data.

2. Broken Access Control:
   Access control refers a system that controls access to information or functionality. Broken access controls allow attackers to bypass authorization and perform tasks as though they were privileged users such as administrators. For example a web application could allow a user to change which account they are logged in as simply by changing part of a url, without any other verification.

Access controls can be secured by ensuring that a web application uses authorization tokens\* and sets tight controls on them.

Many services issue authorization tokens when users log in. Every privileged request that a user makes will require that the authorization token be present. This is a secure way to ensure that the user is who they say they are, without having to constantly enter their login credentials.

3. Broken Authentication:
   Vulnerabilities in authentication (login) systems can give attackers access to user accounts and even the ability to compromise an entire system using an admin account. For example, an attacker can take a list containing thousands of known username/password combinations obtained during a data breach and use a script to try all those combinations on a login system to see

Ques 3: What is the difference between a process and a thread?

Process: 1. An executing instance of a program is called a process. 2. Some operating systems use the term ‘task‘ to refer to a program that is being executed. 3. A process is always stored in the main memory also termed as the primary memory or random access memory. 4. Therefore, a process is termed as an active entity. It disappears if the machine is rebooted. 5. Several process may be associated with a same program.

Thread: 1. A thread is a subset of the process. 2. It is termed as a ‘lightweight process’, since it is similar to a real process but executes within the context of a process and shares the same resources allotted to the process by the kernel. 3. Usually, a process has only one thread of control – one set of machine instructions executing at a time. 4. A process may also be made up of multiple threads of execution that execute instructions concurrently. 5. All the threads running within a process share the same address space, file descriptors, stack and other process related attributes. 8. Since the threads of a process share the same memory, synchronizing the access to the shared data within the process gains unprecedented importance.

Ques2: How do you stop a DDoS attack? 1.
Answer:
Identify the DDoS attack early If you run your own servers, then you need to be able to identify when you are under attack. That’s because the sooner you can establish that problems with your website are due to a DDoS attack, the sooner you can stop the DDoS attack.

        It’s also a good idea to nominate a DDoS leader in your company who is responsible for acting should you come under attack.

    2. Overprovision bandwidth
        It generally makes sense to have more bandwidth available to your Web server than you ever think you are likely to need. That way, you can accommodate sudden and unexpected surges in traffic that could be a result of an advertising campaign, a special offer or even a mention of your company in the media.

        Even if you overprovision by 100 percent — or 500 percent — that likely won’t stop a DDoS attack. But it may give you a few extra minutes to act before your resources are overwhelmed completely.

    3. Defend at the network perimeter (if you run your own web server)
        There are a few technical measures that can be taken to partially mitigate the effect of an attack — especially in the first minutes — and some of these are quite simple.


    4. Call your ISP or hosting provider
        The next step is to call your ISP (or hosting provider if you do not host your own Web server), tell them you are under attack, and ask for help. Keep emergency contacts for your ISP or hosting provider readily available so you can do this quickly. Depending on the strength of the attack, the ISP or hoster may already have detected it – or they may themselves start to be overwhelmed by the attack.

        You stand a better chance of withstanding a DDoS attack if your Web server is located in a hosting center than if you run it yourself. That’s because its data center will likely have far higher bandwidth links and higher capacity routers than your company has, and its staff will probably have more experience dealing with attacks. Having your Web server located with a hoster will also keep DDoS traffic aimed at your Web server off your corporate LAN so at least that part of your business – including email and possibly voice over IP (VoIP) services – should operate normally during an attack.

Ques 3: What is the CAP theorem? Give examples of each.

    Answer: The CAP Theorem states that, in a distributed system (a collection of interconnected nodes that share data.), you can only have two out of the following three guarantees across a write/read pair: Consistency, Availability, and Partition Tolerance - one of them must be sacrificed. However, as you will see below, you don't have as many options here as you might think.

        Consistency - A read is guaranteed to return the most recent write for a given client.
        Availability - A non-failing node will return a reasonable response within a reasonable amount of time (no error or timeout).
        Partition Tolerance - The system will continue to function when network partitions occur.

    the cap theorem categorizes systems into three categories:

    1. cp (consistent and partition tolerant) — at first glance, the cp category is confusing, i.e., a system that is consistent and partition tolerant but never available. cp is referring to a category of systems where availability is sacrificed only in the case of a network partition.

    2. ca (consistent and available) — ca systems are consistent and available systems in the absence of any network partition. often a single node's db servers are categorized as ca systems. single node db servers do not need to deal with partition tolerance and are thus considered ca systems. the only hole in this theory is that single node db systems are not a network of shared data systems and thus do not fall under the preview of cap. [^11]

    3. ap (available and partition tolerant) — these are systems that are available and partition tolerant but cannot guarantee consistency.

Ques 4: What Unix/Linux commands will alter a files ownership, files permissions?

    Answer: Files ownership can be changed using the chown and chgrp commands.
            Files permission can be changed using the following command given below:
                ->chmod g+w filename
                ->chmod g-wx filename
                ->chmod o+w filename
                ->chmod o-rwx foldername

Ques 5:- Differentiate between multithreading and asynchronous.

    -> Asynchronous, single threaded: you start the eggs cooking and set a timer. You start the toast cooking, and set a timer. While they are both cooking, you clean the kitchen. When the timers go off you take the eggs off the heat and the toast out of the toaster and serve them.

    -> Asynchronous, multithreaded: you hire two more cooks, one to cook eggs and one to cook toast. Now you have the problem of coordinating the cooks so that they do not conflict with each other in the kitchen when sharing resources. And you have to pay them.

Threading is about workers, asynchrony is about tasks. In multithreaded workflows you assign tasks to workers. In asynchronous single-threaded workflows you have a graph of tasks where some tasks depend on the results of others; as each task completes it invokes the code that schedules the next task that can run, given the results of the just-completed task.

Ques 6: Differentiate between SQL and No-SQL.

    Answer: The Main Differences:-
    1. Type –
        SQL databases are primarily called as Relational Databases (RDBMS); whereas NoSQL database are primarily called as non-relational or distributed database.

    2. Language –
        SQL databases defines and manipulates data based structured query language (SQL). Seeing from a side this language is extremely powerful. SQL is one of the most versatile and widely-used options available which makes it a safe choice especially for great complex queries. But from other side it can be restrictive. SQL requires you to use predefined schemas to determine the structure of your data before you work with it. Also all of your data must follow the same structure. This can require significant up-front preparation which means that a change in the structure would be both difficult and disruptive to your whole system.

        A NoSQL database has dynamic schema for unstructured data. Data is stored in many ways which means it can be document-oriented, column-oriented, graph-based or organized as a KeyValue store. This flexibility means that documents can be created without having defined structure first. Also each document can have its own unique structure. The syntax varies from database to database, and you can add fields as you go.

    3. The Scalability –
        In almost all situations SQL databases are vertically scalable. This means that you can increase the load on a single server by increasing things like RAM, CPU or SSD. But on the other hand NoSQL databases are horizontally scalable. This means that you handle more traffic by sharding, or adding more servers in your NoSQL database. It is similar to adding more floors to the same building versus adding more buildings to the neighborhood. Thus NoSQL can ultimately become larger and more powerful, making these databases the preferred choice for large or ever-changing data sets.

    4. The Structure –
        SQL databases are table-based on the other hand NoSQL databases are either key-value pairs, document-based, graph databases or wide-column stores. This makes relational SQL databases a better option for applications that require multi-row transactions such as an accounting system or for legacy systems that were built for a relational structure.

    5. Property followed –
        SQL databases follow ACID properties (Atomicity, Consistency, Isolation and Durability) whereas the NoSQL database follows the Brewers CAP theorem (Consistency, Availability and Partition tolerance).

    6. Support –
        Great support is available for all SQL database from their vendors. Also a lot of independent consultations are there who can help you with SQL database for a very large scale deployments but for some NoSQL database you still have to rely on community support and only limited outside experts are available for setting up and deploying your large scale NoSQL deployments.

Ques 7: What is the difference between hardLink and the symlinks.What happens when you
remove the source to a symlink/hardlink?

Answer:- Points to Consider,

        1. A symbolic link does not contain the data in the target file. 2. A symbolic points to another entry somewhere in the file system.
        2. A symbolic has the ability to link to directories, or to files on remote computers networked through NFS.
        3. Deleting a target file for a symbolic link makes that link useless.
        4. A hard link preserves the contents of the file.
        5. A hard link cannot be created for directories, and they cannot cross filesystem boundaries or span across partitions.
        6. In a hardlink you can use any of the hardlink names created to execute a program or script in the same manner as the original name given.
        7. Soft link can span across filesystem.
        8. Soft links can link both files and directories.

    Effects after removing the source of symlinks.
        if the source file is deleted,
            Symlinks:- symlink of that file no longer works or it becomes “dangling link” which points to nonexistent file .
            Hardlinks:- the hard link still works and you will be able to access the file until the number of hard links to file isn’t 0(zero).
