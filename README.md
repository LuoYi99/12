# 12
算法12题
/*
题目:
小明在X星球的城堡中发现了如下图形和文字：
rank=3
   * 
  * * 
 *   *  
* * * *


rank=5
               *                                                      
              * *                                                     
             *   *                                                    
            * * * *                                                   
           *       *                                                  
          * *     * *                                                 
         *   *   *   *                                                
        * * * * * * * *                                               
       *               *                                              
      * *             * *                                             
     *   *           *   *                                            
    * * * *         * * * *                                           
   *       *       *       *  
  * *     * *     * *     * *  
 *   *   *   *   *   *   *   * 
* * * * * * * * * * * * * * * *  


ran=6
                               *                                      
                              * *                                     
                             *   *                                    
                            * * * *                                   
                           *       *                                  
                          * *     * *                                 
                         *   *   *   *                                
                        * * * * * * * *                               
                       *               *                              
                      * *             * *                             
                     *   *           *   *                            
                    * * * *         * * * *                           
                   *       *       *       *                          
                  * *     * *     * *     * *                         
                 *   *   *   *   *   *   *   *                        
                * * * * * * * * * * * * * * * *                       
               *                               *                      
              * *                             * *                     
             *   *                           *   *                    
            * * * *                         * * * *                   
           *       *                       *       *                  
          * *     * *                     * *     * *                 
         *   *   *   *                   *   *   *   *                
        * * * * * * * *                 * * * * * * * *               
       *               *               *               *              
      * *             * *             * *             * *             
     *   *           *   *           *   *           *   *            
    * * * *         * * * *         * * * *         * * * *           
   *       *       *       *       *       *       *       *          
  * *     * *     * *     * *     * *     * *     * *     * *         
 *   *   *   *   *   *   *   *   *   *   *   *   *   *   *   *        
* * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * *       

*/
/*
思路：
动态创建二维数组
从图中可找出规律
每次打印rank=n的图时
等价于打印三个rank=n-1的图
只是这三个图按照一定位置摆放
所以
利用二维数组实现快速摆放
摆放完后打印图片

*/
