module design_1
   (bias,
    bias_1,
    bias_2,
    bias_3,
    clk,
    in1,
    in1_1,
    in1_2,
    in1_3,
    in2,
    in2_1,
    in2_2,
    in2_3,
    in3,
    in3_1,
    in3_2,
    in3_3,
    in4,
    in4_1,
    in4_2,
    in4_3,
    mac,
    n_en,
    n_in,
    n_in_1,
    n_in_2,
    n_in_3,
    n_out,
    n_out_1,
    n_out_2,
    n_out_3,
    outen,
    outen_1,
    outen_2,
    outen_3,
    p_en,
    p_out,
    p_out_1,
    p_out_2,
    p_out_3,
    rst,
    wgh,
    wgh_1,
    wgh_2,
    wgh_3);
  input [15:0]bias;
  input [15:0]bias_1;
  input [15:0]bias_2;
  input [15:0]bias_3;
  input clk;
  input [15:0]in1;
  input [15:0]in1_1;
  input [15:0]in1_2;
  input [15:0]in1_3;
  input [15:0]in2;
  input [15:0]in2_1;
  input [15:0]in2_2;
  input [15:0]in2_3;
  input [15:0]in3;
  input [15:0]in3_1;
  input [15:0]in3_2;
  input [15:0]in3_3;
  input [15:0]in4;
  input [15:0]in4_1;
  input [15:0]in4_2;
  input [15:0]in4_3;
  input mac;
  input n_en;
  input [15:0]n_in;
  input [15:0]n_in_1;
  input [15:0]n_in_2;
  input [15:0]n_in_3;
  output [15:0]n_out;
  output [15:0]n_out_1;
  output [15:0]n_out_2;
  output [15:0]n_out_3;
  output outen;
  output outen_1;
  output outen_2;
  output outen_3;
  input p_en;
  output [15:0]p_out;
  output [15:0]p_out_1;
  output [15:0]p_out_2;
  output [15:0]p_out_3;
  input rst;
  input [15:0]wgh;
  input [15:0]wgh_1;
  input [15:0]wgh_2;
  input [15:0]wgh_3;

  wire [15:0]\^bias_1 ;
  wire [15:0]bias_1_1;
  wire [15:0]bias_2_1;
  wire [15:0]bias_3_1;
  wire clk_1;
  wire en_1;
  wire en_2;
  wire [15:0]\^in1_1 ;
  wire [15:0]in1_1_1;
  wire [15:0]in1_2_1;
  wire [15:0]in1_3_1;
  wire [15:0]\^in2_1 ;
  wire [15:0]in2_1_1;
  wire [15:0]in2_2_1;
  wire [15:0]in2_3_1;
  wire [15:0]\^in3_1 ;
  wire [15:0]in3_1_1;
  wire [15:0]in3_2_1;
  wire [15:0]in3_3_1;
  wire [15:0]\^in4_1 ;
  wire [15:0]in4_1_1;
  wire [15:0]in4_2_1;
  wire [15:0]in4_3_1;
  wire mac_1;
  wire [15:0]\^n_in_1 ;
  wire [15:0]n_in_1_1;
  wire [15:0]n_in_2_1;
  wire [15:0]n_in_3_1;
  wire [15:0]neuron_0_n_out;
  wire [15:0]neuron_1_n_out;
  wire [15:0]neuron_2_n_out;
  wire [15:0]neuron_3_n_out;
  wire pooling_0_outen;
  wire [15:0]pooling_0_p_out;
  wire pooling_1_outen;
  wire [15:0]pooling_1_p_out;
  wire pooling_2_outen;
  wire [15:0]pooling_2_p_out;
  wire pooling_3_outen;
  wire [15:0]pooling_3_p_out;
  wire rst_1;
  wire [15:0]\^wgh_1 ;
  wire [15:0]wgh_1_1;
  wire [15:0]wgh_2_1;
  wire [15:0]wgh_3_1;

  assign \^bias_1 [15:0] = bias[15:0];
  assign \^in1_1 [15:0] = in1[15:0];
  assign \^in2_1 [15:0] = in2[15:0];
  assign \^in3_1 [15:0] = in3[15:0];
  assign \^in4_1 [15:0] = in4[15:0];
  assign \^n_in_1 [15:0] = n_in[15:0];
  assign \^wgh_1 [15:0] = wgh[15:0];
  assign bias_1_1 = bias_1[15:0];
  assign bias_2_1 = bias_2[15:0];
  assign bias_3_1 = bias_3[15:0];
  assign clk_1 = clk;
  assign en_1 = n_en;
  assign en_2 = p_en;
  assign in1_1_1 = in1_1[15:0];
  assign in1_2_1 = in1_2[15:0];
  assign in1_3_1 = in1_3[15:0];
  assign in2_1_1 = in2_1[15:0];
  assign in2_2_1 = in2_2[15:0];
  assign in2_3_1 = in2_3[15:0];
  assign in3_1_1 = in3_1[15:0];
  assign in3_2_1 = in3_2[15:0];
  assign in3_3_1 = in3_3[15:0];
  assign in4_1_1 = in4_1[15:0];
  assign in4_2_1 = in4_2[15:0];
  assign in4_3_1 = in4_3[15:0];
  assign mac_1 = mac;
  assign n_in_1_1 = n_in_1[15:0];
  assign n_in_2_1 = n_in_2[15:0];
  assign n_in_3_1 = n_in_3[15:0];
  assign n_out[15:0] = neuron_3_n_out;
  assign n_out_1[15:0] = neuron_0_n_out;
  assign n_out_2[15:0] = neuron_1_n_out;
  assign n_out_3[15:0] = neuron_2_n_out;
  assign outen = pooling_0_outen;
  assign outen_1 = pooling_1_outen;
  assign outen_2 = pooling_2_outen;
  assign outen_3 = pooling_3_outen;
  assign p_out[15:0] = pooling_0_p_out;
  assign p_out_1[15:0] = pooling_1_p_out;
  assign p_out_2[15:0] = pooling_2_p_out;
  assign p_out_3[15:0] = pooling_3_p_out;
  assign rst_1 = rst;
  assign wgh_1_1 = wgh_1[15:0];
  assign wgh_2_1 = wgh_2[15:0];
  assign wgh_3_1 = wgh_3[15:0];
  neuron neuron_0
       (.bias(bias_1_1),
        .clk(clk_1),
        .en(en_1),
        .mac(mac_1),
        .n_in(n_in_1_1),
        .n_out(neuron_0_n_out),
        .rst(rst_1),
        .wgh(wgh_1_1));
  neuron neuron_1
       (.bias(bias_2_1),
        .clk(clk_1),
        .en(en_1),
        .mac(mac_1),
        .n_in(n_in_2_1),
        .n_out(neuron_1_n_out),
        .rst(rst_1),
        .wgh(wgh_2_1));
  neuron neuron_2
       (.bias(bias_3_1),
        .clk(clk_1),
        .en(en_1),
        .mac(mac_1),
        .n_in(n_in_3_1),
        .n_out(neuron_2_n_out),
        .rst(rst_1),
        .wgh(wgh_3_1));
  neuron neuron_3
       (.bias(\^bias_1 ),
        .clk(clk_1),
        .en(en_1),
        .mac(mac_1),
        .n_in(\^n_in_1 ),
        .n_out(neuron_3_n_out),
        .rst(rst_1),
        .wgh(\^wgh_1 ));
  pooling pooling_0
       (.clk(clk_1),
        .en(en_2),
        .in1(\^in1_1 ),
        .in2(\^in2_1 ),
        .in3(\^in3_1 ),
        .in4(\^in4_1 ),
        .outen(pooling_0_outen),
        .p_out(pooling_0_p_out));
  pooling pooling_1
       (.clk(clk_1),
        .en(en_2),
        .in1(in1_1_1),
        .in2(in2_1_1),
        .in3(in3_1_1),
        .in4(in4_1_1),
        .outen(pooling_1_outen),
        .p_out(pooling_1_p_out));
  pooling pooling_2
       (.clk(clk_1),
        .en(en_2),
        .in1(in1_2_1),
        .in2(in2_2_1),
        .in3(in3_2_1),
        .in4(in4_2_1),
        .outen(pooling_2_outen),
        .p_out(pooling_2_p_out));
  pooling pooling_3
       (.clk(clk_1),
        .en(en_2),
        .in1(in1_3_1),
        .in2(in2_3_1),
        .in3(in3_3_1),
        .in4(in4_3_1),
        .outen(pooling_3_outen),
        .p_out(pooling_3_p_out));
endmodule
module neuron(
input [15:0] n_in,
input [15:0] wgh,
input [15:0] bias,
input clk,
input en,
input rst,
input mac,
output reg [15:0] n_out

    );
    
    reg [29:0] t;
    reg [15:0] temp;
    reg [15:0] sum;
    reg [15:0] tsum;
    
    
    always@(posedge clk)
    begin
    if(rst)
    begin
       n_out<=0;
       sum<=0;
       temp<=0;
       t<=0;
       tsum<=0;
    end
    else if(en)
         begin
	    if(en && mac)
       begin
          tsum<=sum+bias;
                       if(sum[14:0]>bias[14:0])
                       begin
                           if(bias[15]&&sum[15])
                           begin
                              if(!tsum[15])
                              begin
                                 sum<=16'b1111111110000000;
                              end
                              else sum<={1'b1,(sum[14:0]+bias[14:0])}; 
                           end
                           else if(bias[15]&&(!sum[15]))
                           begin
                              sum<={1'b0,(sum[14:0]-bias[14:0])};
                           end
                           else if((!bias[15])&&sum[15])
                           begin
                               sum<={1'b1,(sum[14:0]-bias[14:0])};
                           end
                           else
                           begin
                              if(tsum[15])
                              begin
                                 sum<=16'b0111111110000000;
                              end
                              else sum<={1'b0,(sum[14:0]+bias[14:0])};
                           end
                       end
                       else if(sum[14:0]<bias[14:0])
                       begin
                          if(bias[15]&&sum[15])
                          begin
                             if(!tsum[15])
                             begin
                                sum<=16'b1111111110000000;
                             end
                             else sum<={1'b1,(sum[14:0]+bias[14:0])}; 
                          end
                          else if(bias[15]&&(!sum[15]))
                          begin
                             sum<={1'b1,(bias[14:0]-sum[14:0])};
                          end
                          else if((!bias[15])&&sum[15])
                          begin
                             sum<={1'b0,(bias[14:0]-sum[14:0])};
                          end
                          else
                          begin
                             if(tsum[15])
                             begin
                                sum<=16'b0111111110000000;
                             end
                             else sum<={1'b0,(sum[14:0]+bias[14:0])};
                          end
                       end
                       
                       
                       if(sum[15])
                       begin
                          n_out<=0;
                       end
                       else
                       begin
                          n_out<=sum;
                       end
       end
            else if(!mac)
            begin
                t<=n_in[14:0]*wgh[14:0];
                if(n_in[15]^wgh[15])
                begin
                    temp<={1'b1,t[21:7]};
                end
                else
                begin
                    temp<={1'b0,t[21:7]};
                end
                tsum<=sum+temp;
                if(sum[14:0]>temp[14:0])
                begin
                    if(temp[15]&&sum[15])
                    begin
                       if(!tsum[15])
                       begin
                          sum<=16'b1111111110000000;
                       end
                       else sum<={1'b1,(sum[14:0]+temp[14:0])}; 
                    end
                    else if(temp[15]&&(!sum[15]))
                    begin
                       sum<={1'b0,(sum[14:0]-temp[14:0])};
                    end
                    else if((!temp[15])&&sum[15])
                    begin
                        sum<={1'b1,(sum[14:0]-temp[14:0])};
                    end
                    else
                    begin
                       if(tsum[15])
                       begin
                          sum<=16'b0111111110000000;
                       end
                       else sum<={1'b0,(sum[14:0]+temp[14:0])};
                    end
                end
                else if(sum[14:0]<temp[14:0])
                begin
                   if(temp[15]&&sum[15])
                   begin
                      if(!tsum[15])
                      begin
                         sum<=16'b1111111110000000;
                      end
                      else sum<={1'b1,(sum[14:0]+temp[14:0])}; 
                   end
                   else if(temp[15]&&(!sum[15]))
                   begin
                      sum<={1'b1,(temp[14:0]-sum[14:0])};
                   end
                   else if((!temp[15])&&sum[15])
                   begin
                      sum<={1'b0,(temp[14:0]-sum[14:0])};
                   end
                   else
                   begin
                      if(tsum[15])
                      begin
                         sum<=16'b0111111110000000;
                      end
                      else sum<={1'b0,(sum[14:0]+temp[14:0])};
                   end
                end               
            end
         end
    end
    
//    always@ (posedge clk)
//    begin
//       out<=sum;
//    end
    
/*   always @(posedge clk)
    begin
       if(en && mac)
       begin
          tsum<=sum+bias;
                       if(sum[14:0]>bias[14:0])
                       begin
                           if(bias[15]&&sum[15])
                           begin
                              if(!tsum[15])
                              begin
                                 sum<=16'b1111111110000000;
                              end
                              else sum<={1'b1,(sum[14:0]+bias[14:0])}; 
                           end
                           else if(bias[15]&&(!sum[15]))
                           begin
                              sum<={1'b0,(sum[14:0]-bias[14:0])};
                           end
                           else if((!bias[15])&&sum[15])
                           begin
                               sum<={1'b1,(sum[14:0]-bias[14:0])};
                           end
                           else
                           begin
                              if(tsum[15])
                              begin
                                 sum<=16'b0111111110000000;
                              end
                              else sum<={1'b0,(sum[14:0]+bias[14:0])};
                           end
                       end
                       else if(sum[14:0]<bias[14:0])
                       begin
                          if(bias[15]&&sum[15])
                          begin
                             if(!tsum[15])
                             begin
                                sum<=16'b1111111110000000;
                             end
                             else sum<={1'b1,(sum[14:0]+bias[14:0])}; 
                          end
                          else if(bias[15]&&(!sum[15]))
                          begin
                             sum<={1'b1,(bias[14:0]-sum[14:0])};
                          end
                          else if((!bias[15])&&sum[15])
                          begin
                             sum<={1'b0,(bias[14:0]-sum[14:0])};
                          end
                          else
                          begin
                             if(tsum[15])
                             begin
                                sum<=16'b0111111110000000;
                             end
                             else sum<={1'b0,(sum[14:0]+bias[14:0])};
                          end
                       end
                       
                       
                       if(sum[15])
                       begin
                          n_out<=0;
                       end
                       else
                       begin
                          n_out<=sum;
                       end
       end
    end
*/
endmodule
module pooling(
input clk,
input [15:0] in1,
input [15:0] in2,
input [15:0] in3,
input [15:0] in4,
input en,
output reg [15:0] p_out,
output reg outen

    );
    
   parameter inimax= 16'b000000000000000;
   always @ (posedge clk) begin
           if(en) begin
               if(inimax < (in1)) begin
                   if((in2) < (in1)) begin
                       if((in3) < (in1)) begin
                           if((in4) < (in1)) begin
                               p_out <= in1;
                               outen <= 1;
                           end
                           else begin
                               p_out <= in4;
                               outen <= 1;
                           end
                       end
                       else begin
                           if((in3) < (in4)) begin
                               p_out <= in4;
                               outen <= 1;
                           end
                           else begin
                               p_out <= in3;
                               outen <= 1;
                           end
                       end
                   end
                   else begin
                       if((in3) < (in2)) begin
                           if((in4) < (in2)) begin
                               p_out <= in2;
                               outen <= 1;
                           end
                           else begin
                               p_out <= in4;
                               outen <= 1;
                           end
                       end
                       else begin
                           if((in3) < (in4)) begin
                               p_out <= in4;
                               outen <= 1;
                           end
                           else begin
                               p_out <= in3;
                               outen <= 1;
                           end
                       end
                   end
               end
               else begin
                   p_out <= inimax;
                   outen <= 1;
               end
           end
           else begin
               p_out <= 0;
               outen <= 0;
           end
       end

endmodule
