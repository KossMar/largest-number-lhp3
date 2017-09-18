# largest-number-lhp3
Lighthouse Prep Assignment 3


#import <Foundation/Foundation.h>
#import "LargestNumber.h"

int main(int argc, const char * argv[]) {
    @autoreleasepool {
       
        
        
        NSArray *unsorted = @[@30, @20, @9, @103, @249, @20];
        NSArray *unsorted2 = @[@50, @53, @79, @55, @62, @07, @78];

        
        [LargestNumber findLargest:unsorted];
        [LargestNumber findLargest:unsorted2];
        
        
        
     
        }
        
    return 0;
}
