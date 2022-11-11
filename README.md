pip install pytest
from serpapi import GoogleSearch
import os, json
image_results = []

for query in ["Headboards & Footboards"]:
    params = {
        "engine": "google",               # Google Search Engine 
        "q": query,                       # search query Details 
        "tbm": "isch",                    # image results
        "num": "100",                     # number of images per page
        "ijn": 0,                         # page number: 0 -> first page, 1 -> second...
        "api_key":("36363613acf21eaeeae1fc471178bb7af0d63e3a1b4c4e9034d0bc57673cab4e")   # your serpapi api key
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
          for image in results["images_results"]:
            if image["original"] not in image_results:
              print(image["original"])
              image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
-----------------------------------------------------------------------------------------
image_results = []

for query in ["Bed Frames"]:
    params = {
        "engine": "google",              
        "q": query,                       
        "tbm": "isch",                    
        "num": "100",                     
        "ijn": 0,                        
        "api_key":("36363613acf21eaeeae1fc471178bb7af0d63e3a1b4c4e9034d0bc57673cab4e")   
    }

    search = GoogleSearch(params)        
    images_is_present = True
    while images_is_present:
        results = search.get_dict()       

      
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
-----------------------------------------------------------------------
image_results = []

for query in ["Bedroom Sets"]:
    params = {
        "engine": "google",               
        "q": query,                      
        "tbm": "isch",                   
        "num": "100",                  
        "ijn": 0,                         
        "api_key":("36363613acf21eaeeae1fc471178bb7af0d63e3a1b4c4e9034d0bc57673cab4e")   
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
-----------------------------------------------------------------
image_results = []

for query in ["Bedding"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                    
        "num": "100",                     
        "ijn": 0,                         
        "api_key":("36363613acf21eaeeae1fc471178bb7af0d63e3a1b4c4e9034d0bc57673cab4e")   
    }

    search = GoogleSearch(params)         # where data extraction happens

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       # JSON -> Python dictionary

        # checks for "Google hasn't returned any results for this query."
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            # update to the next page
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
--------------------------------------------------------------------
image_results = []

for query in ["Mattresses"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                    
        "num": "100",                     
        "ijn": 0,                         
        "api_key":("36363613acf21eaeeae1fc471178bb7af0d63e3a1b4c4e9034d0bc57673cab4e")   
    }

    search = GoogleSearch(params)         

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       

       
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
--------------------------------------------------------------------------
image_results = []

for query in ["Nightstands"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                    
        "num": "100",                     
        "ijn": 0,                         
        "api_key":("36363613acf21eaeeae1fc471178bb7af0d63e3a1b4c4e9034d0bc57673cab4e")   
    }

    search = GoogleSearch(params)         

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       

        
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
-------------------------------------------------------------------------
image_results = []

for query in ["Dressers"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                    
        "num": "100",                    
        "ijn": 0,                         
        "api_key":("36363613acf21eaeeae1fc471178bb7af0d63e3a1b4c4e9034d0bc57673cab4e")   
    }

    search = GoogleSearch(params)         

    images_is_present = True
    while images_is_present:
        results = search.get_dict()      

        
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
-------------------------------------------------------------------------
image_results = []

for query in ["Vanities"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                   
        "num": "100",                     
        "ijn": 0,                         
        "api_key":("36363613acf21eaeeae1fc471178bb7af0d63e3a1b4c4e9034d0bc57673cab4e")   
    }

    search = GoogleSearch(params)         

    images_is_present = True
    while images_is_present:
        results = search.get_dict()      

        
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
--------------------------------------------------------------------------
image_results = []

for query in ["Wall Art"]:
    params = {
        "engine": "google",               
        "q": query,                       
        "tbm": "isch",                   
        "num": "100",                     
        "ijn": 0,                         # 
        "api_key":("36363613acf21eaeeae1fc471178bb7af0d63e3a1b4c4e9034d0bc57673cab4e")   
    }

    search = GoogleSearch(params)         

    images_is_present = True
    while images_is_present:
        results = search.get_dict()       

        
        if "error" not in results:
            for image in results["images_results"]:
                if image["original"] not in image_results:
                    print(image["original"])
                    image_results.append(image["original"])
            
            
            params["ijn"] += 1
        else:
            images_is_present = False
            print(results["error"])

print(json.dumps(image_results, indent=2))
print(len(image_results))
