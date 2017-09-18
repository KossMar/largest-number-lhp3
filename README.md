# largest-number-lhp3
Lighthouse Prep Assignment 3


#import <Foundation/Foundation.h>
#import "LargestNumber.h"

@interface LargestNumber : NSObject

+(id)findLargest:(NSArray*)array;

@end

@implementation LargestNumber

+(id) findLargest:(NSArray*) array {
    
    
    NSString *foo = array[0];
    for (int i = 0; i < array.count; i++) {
        foo = foo > array[i] ? foo : array[i];
    }
    NSLog(@"Largest Number %@", foo);
    return foo;
    }


@end


int main(int argc, const char * argv[]) {
    @autoreleasepool {
       
        
        
        NSArray *unsorted = @[@30, @20, @9, @103, @249, @20];
        NSArray *unsorted2 = @[@50, @53, @79, @55, @62, @07, @78];

        
        [LargestNumber findLargest:unsorted];
        [LargestNumber findLargest:unsorted2];
        
        
        
     
        }
        
    return 0;
}
