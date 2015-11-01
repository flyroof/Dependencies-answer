# Dependencies-answer

By Blaga

Here is a possible part of the solution in Java.

package jetbrains;

import java.util.Scanner;

import org.json.simple.JSONObject;

public class Dependencies

{

public static void main(String[] args) 

{
    Scanner input = new Scanner(System.in);
    System.out.println("Installing backbone.");
    JSONObject backbone = new JSONObject();
    System.out.println("In order to install backbone, we need jQuery and underscore.");
    backbone.put("jQuery", "underscore");
    System.out.println("Installing JQuery");
    JSONObject JQuery = new JSONObject();

    System.out.println("In order to install JQuery, we need queryJ.");
    JQuery.putIfAbsent("queryJ", args);

    JSONObject underscore = new JSONObject();
    underscore.putIfAbsent("lodash", args);

    System.out.println("Installing queryJ.");
    JSONObject queryJ = new JSONObject();
    queryJ.putIfAbsent(args, args);

    JSONObject lodash = new JSONObject();
    lodash.putIfAbsent(args, args);
    System.out.println("Installing underscore.");
    System.out.println("In order to install underscore, we need lodash. Lodash is already installed.");
    System.out.println("All done.");

}

}
