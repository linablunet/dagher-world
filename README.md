# dagher-world
import com.google.android.gms.ads.AdRequest;
import com.google.android.gms.ads.AdView;
// ...


public class MainActivity extends AppCompatActivity {

    private AdView mAdView;
    // ...

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        mAdView = (AdView) findViewById(R.id.adView);
        AdRequest adRequest = new AdRequest.Builder().build();
        mAdView.loadAd(adRequest);
