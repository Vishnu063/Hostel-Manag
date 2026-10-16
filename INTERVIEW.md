# Hostel management application — fork: reviewer guide

A fork of a Java servlet/JSP application with DAO and entity layers.

## Start the review

Separate inherited application code from your own changes. Explain database connections, request handling, and WAR packaging.

| Source | Review focus |\n| --- | --- |\n| [pom.xml](pom.xml) | Implementation, assumptions, and operational boundaries |\n| [src/main/java/com/smarthostel/ConnectionFactory/DBConnection.java](src/main/java/com/smarthostel/ConnectionFactory/DBConnection.java) | Implementation, assumptions, and operational boundaries |\n| [src/main/java/com/smarthostel/dao/ComplaintDAO.java](src/main/java/com/smarthostel/dao/ComplaintDAO.java) | Implementation, assumptions, and operational boundaries |\n| [src/main/java/com/smarthostel/dao/FeeDAO.java](src/main/java/com/smarthostel/dao/FeeDAO.java) | Implementation, assumptions, and operational boundaries |\n| [src/main/java/com/smarthostel/dao/RoomDAO.java](src/main/java/com/smarthostel/dao/RoomDAO.java) | Implementation, assumptions, and operational boundaries |\n| [src/main/java/com/smarthostel/dao/StudentDAO.java](src/main/java/com/smarthostel/dao/StudentDAO.java) | Implementation, assumptions, and operational boundaries |

## A useful interview walkthrough

1. State the problem and the specific part you implemented or changed.
2. Open the source above and follow one request, release, or failure from start to finish.
3. Show a reproducible result, including an actual failure and the observation that confirms recovery.
4. Explain one tradeoff and one limitation. Distinguish a local test from a live deployment.

## Evidence and limits

This guide is based on the default-branch source inspected on 16 October 2026. It is a source review, not a fresh deployment or a certification of every feature. Existing CI runs and tests should be checked at the commit being demonstrated. Do not present screenshots, inherited code, planned features, or old README statements as proof of a current deployment.

## Attribution

This repository is a fork of [shubham93096/HostelManagment1](https://github.com/shubham93096/HostelManagment1). The application and existing documentation retain their original authorship. Use commit diffs to identify any changes made in this fork; no original authorship or completed deployment is implied.
