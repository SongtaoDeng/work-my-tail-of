# work-my-tail-of
#Where there is a will there is a way
#for 1-100所有素数 每6个换行
//输出1-1000的所有素数，并且每6个换行
//知识点：count统计 boolean 标记 break 以及for循环这个一定要独立完成！
public class ForTest10 {
    public static void main(String[] args) {
        int count = 0;
        for (int i = 2; i < 1000; i++) {
            boolean isSuShu = true;
            for (int j = 2; j < i; j++) {
                if (i % j == 0) {
                    isSuShu = false;
                    break;

                }

            }
            if (isSuShu) {
                System.out.print(i + " ");
                count++;
                if (count % 6 == 0) {
                    System.out.println("");
                }

            }
        }
    }
}
